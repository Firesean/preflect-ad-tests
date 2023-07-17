<script>
    import CreateAdButton from '$lib/components/create_ad_button.svelte';
    import AdCard from '$lib/components/ad_card.svelte';
    import SideNav from '$lib/components/side_nav.svelte';


</script>

<div class='w-3/4 flex ml-auto'>
    <div>    
        <h1 class='font-bold text-3xl'>Meta Ads</h1>
        <p class='flex text-gray-one text-base'>Run evergreen ads on Facebook and Instagram</p>
    </div>
    <CreateAdButton />
</div>

<section class='w-3/4 flex ml-auto'>
    <AdCard />
</section>