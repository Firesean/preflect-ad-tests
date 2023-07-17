<script>
    import CreateAdButton from '$lib/components/create_ad_button.svelte';
    import AdCard from '$lib/components/ad_card.svelte';
</script>

<div class='w-3/4 ml-auto grid bg-gray-two p-3'>
    <div class="grid grid-cols-2">
        <div class='p-2 m-auto'>
            <h1 class='font-bold text-3xl'>Meta Ads</h1>
            <p class='text-gray-one text-base'>Run evergreen ads on Facebook and Instagram</p>
        </div>
        <div class="col-start-2 grid justify-end">
            <CreateAdButton />
        </div>
    </div>
    <section class="grid grid-cols-3">
        <AdCard />
        <AdCard />
        <AdCard />
        <AdCard />
        <AdCard />
        <AdCard />
        <AdCard />
        <AdCard />
        <AdCard />
    </section>
</div>