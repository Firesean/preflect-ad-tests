<script>
  import ToggleButton from "./ToggleButton.svelte";
</script>

<style>
  figure{
    @apply text-gray-two;
  }
</style>

<div class="grid col-span-1 bg-white-one w-[90%] h-[70%] p-2 rounded-lg">
  <svg xmlns="http://www.w3.org/2000/svg" fill="#5650e3" viewBox="0 0 24 24" stroke-width="1.5" stroke="white" class="w-5 h-5">
    <path stroke-linecap="round" stroke-linejoin="round" d="M12 0c6.623 0 12 5.377 12 12s-5.377 12-12 12-12-5.377-12-12 5.377-12 12-12zm0 1c6.071 0 11 4.929 11 11s-4.929 11-11 11-11-4.929-11-11 4.929-11 11-11zm0 11h6v1h-7v-9h1v8z" /> <!-- 3 o'clock SVG -->
  </svg> 
  <span class="justify-end grid text-purple-one font-semibold">edit     
    <ToggleButton />
  </span>

    <div class="grid grid-cols-3 gap-2 w-full">
      <figure class='grid col-span-2 w-[1rem] h-[1rem]'>
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class="rounded-lg h-full" src="../../../src/images/photo-1685226119907-1d836117d2fe.jpg" alt="Placeholder Image">
        <figcaption>Feed</figcaption>
      </figure>

      <figure class='grid col-span-1'>
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class="rounded-lg h-full" src="../../../src/images/photo-1685226119907-1d836117d2fe.jpg" alt="Placeholder Image">
        <figcaption>Story</figcaption>
      </figure>
  </div>
</div>