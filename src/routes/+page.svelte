<script>
    import CreateAdButton from '$lib/components/CreateAdButton.svelte';
    import AdCard from '$lib/components/AdCard.svelte';
</script>

<div class='h-full grid bg-gray-three p-3 pl-[3rem] pr-[3rem] sm:w-full'>
    <div class="grid grid-cols-2 h-[100%] mb-[3rem] mt-[2rem]">
      <div>
        <h1 class='font-bold text-3xl'>Meta Ads</h1>
        <p class='text-gray-one text-base'>Run evergreen ads on Facebook and Instagram</p>
      </div>
      <div class="absolute mt-[1rem] right-[3rem]  w-[7rem] md:w-[9rem] sm:w-[12rem]">
        <CreateAdButton />
      </div>
    </div>
    <section class="grid sm:grid-cols-3 gap-3 mb-[100%]">
      <AdCard feedImg="https://source.unsplash.com/random/?dog" storyImg="https://source.unsplash.com/random/?dog"/>
      <AdCard feedImg="https://source.unsplash.com/random/?mouse" storyImg="https://source.unsplash.com/random/?cat"/>
      <AdCard feedImg="https://source.unsplash.com/random/?snake" storyImg="https://source.unsplash.com/random/?horse"/>
      <AdCard feedImg="https://source.unsplash.com/random/?blue" storyImg="https://source.unsplash.com/random/?computer"/>
    </section>
  </div>
  