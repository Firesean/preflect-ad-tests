<script>
    import CreateAdButton from '$lib/components/CreateAdButton.svelte';
    import AdCard from '$lib/components/AdCard.svelte';

    let objects = ["apple", "banana", "orange", "grape", "kiwi", "boat", "car", "road", "skyscraper", "hockey", "baseball", "dancing", "fun"];
    let adCards = [];

    function createAdCard(){
      let randomIndex = 0;
      console.log("Creating object?");
      const newAd = {feed: randomIndex = Math.floor(Math.random() * objects.length),
                      story: randomIndex = Math.floor(Math.random() * objects.length)};
      adCards = [...adCards, newAd];
    }

</script>

<div class='h-full grid bg-gray-three p-3 pl-[3rem] pr-[3rem] sm:w-full'>
    <div class="grid sm:grid-cols-2 grid-rows-2 h-[100%] mb-[3rem] mt-[2rem]">
      <div>
        <h1 class='font-bold text-3xl'>Meta Ads</h1>
        <p class='text-gray-one text-base'>Run evergreen ads on Facebook and Instagram</p>
      </div>

      <!-- Need to remake the CreateAdButton -->
      <!-- svelte-ignore a11y-no-static-element-interactions -->
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div class="sm:absolute mt-[-1rem] sm:mt-[1rem] right-[3rem] w-[7rem] md:w-[9rem] sm:w-[12rem]" on:click={createAdCard}>
        <CreateAdButton/>
      </div>
    </div>
    <section class="grid mt-[-2rem] sm:mt-[-5rem] sm:grid-cols-3 gap-3 mb-[100%]">
      <AdCard feedImg="https://source.unsplash.com/random/?dog" storyImg="https://source.unsplash.com/random/?dog"/>
      <AdCard feedImg="https://source.unsplash.com/random/?mouse" storyImg="https://source.unsplash.com/random/?cat"/>
      <AdCard feedImg="https://source.unsplash.com/random/?snake" storyImg="https://source.unsplash.com/random/?horse"/>
      <AdCard feedImg="https://source.unsplash.com/random/?blue" storyImg="https://source.unsplash.com/random/?computer"/>
      {#each adCards as ad}
        <AdCard feedImg="https://source.unsplash.com/random/?{objects[ad.feed]}" storyImg="https://source.unsplash.com/random/?{objects[ad.story]}"/>
      {/each}
    </section>
  </div>
  