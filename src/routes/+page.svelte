<script>
    import CreateAdButton from '$lib/components/CreateAdButton.svelte';
    import AdCard from '$lib/components/AdCard.svelte';
</script>

<div class='w-4/5 ml-auto grid bg-gray-three p-3 pl-[3rem]'>
    <div class="grid grid-cols-2 h-[100%]">
        <div>
            <h1 class='font-bold text-3xl'>Meta Ads</h1>
            <p class='text-gray-one text-base'>Run evergreen ads on Facebook and Instagram</p>
        </div>
        <div class="mt-[1rem] ml-[12rem]">
            <CreateAdButton />
        </div>
    </div>
    <section class="grid grid-cols-3">
        <AdCard />
        <AdCard />
        <!-- <AdCard /> -->
        <!-- <AdCard />
        <AdCard />
        <AdCard />
        <AdCard /> -->
    </section>
</div>