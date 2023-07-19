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
      <div class="mt-[1rem]">
        <CreateAdButton />
      </div>
    </div>
    <section class="grid sm:grid-cols-3 gap-3 mb-[100%]">
      <AdCard feedImg="../../../src/images/photo-1685226119907-1d836117d2fe.jpg" storyImg="../../../src/images/premium_photo-1673913966947-a9e2bf8ddf20.jpg"/>
      <AdCard feedImg="../../../src/images/photo-1687463221057-bfb5daae88d0.jpg" storyImg="../../../src/images/photo-1687367480028-e4f582ff92b0.jpg"/>
      <AdCard feedImg="../../../src/images/photo-1687015834172-232445885588.jpg" storyImg="../../../src/images/photo-1687913161653-7cddb0ba09b0.jpg"/>
      <AdCard feedImg="../../../src/images/premium_photo-1684706282813-201f3afb35b6.jpg" storyImg="../../../src/images/photo-1688310482819-fb0ce61f9fcf.jpg"/>
    </section>
  </div>
  