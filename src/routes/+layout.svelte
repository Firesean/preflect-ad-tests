<script>
    import '../app.css';
    import { onMount } from 'svelte';

    let title = 'Preflect Ads';
        onMount(() => {
        document.title = title; // Set the document title on component mount
    });
</script>

<slot />