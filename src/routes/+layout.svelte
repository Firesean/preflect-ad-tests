<script>
    import SideNav from '$lib/components/side_nav.svelte';
    import '../app.css';
    import { onMount } from 'svelte';

    let title = 'Preflect Ads';
        onMount(() => {
        document.title = title; // Set the document title on component mount
    });
</script>

<div class='flex'>
    <SideNav />
    <slot />
</div>