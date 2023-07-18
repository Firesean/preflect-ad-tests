<script>
  import ToggleButton from "./ToggleButton.svelte";
</script>

<style>
  figure{
    @apply text-gray-two;
  }
</style>

<div class="grid col-span-1 bg-white-one w-[100%] h-[100%] p-2 rounded-lg">
  <span class="justify-end grid grid-cols-2 text-purple-one font-semibold">
    <svg xmlns="http://www.w3.org/2000/svg" fill="#5650e3" viewBox="0 0 24 24" stroke-width="1.5" stroke="white" class="w-5 h-5">
      <path stroke-linecap="round" stroke-linejoin="round" d="M12 0c6.623 0 12 5.377 12 12s-5.377 12-12 12-12-5.377-12-12 5.377-12 12-12zm0 1c6.071 0 11 4.929 11 11s-4.929 11-11 11-11-4.929-11-11 4.929-11 11-11zm0 11h6v1h-7v-9h1v8z" /> <!-- 3 o'clock SVG -->
    </svg> 
    <div class="flex flex-row justify-end flex-shrink-0">
      <span class="pr-4">edit</span>
      <ToggleButton />
    </div>
  </span>

    <div class="grid grid-cols-5 gap-2 w-[100%] h-[100%] pb-[3rem]">
      <figure class='grid col-span-3'>
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class="rounded-lg object-cover w-full h-full" src="../../../src/images/photo-1685226119907-1d836117d2fe.jpg" alt="Placeholder Image">
      </figure>

      <figure class='grid col-span-2'>
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class="rounded-lg object-cover w-full h-full" src="../../../src/images/photo-1685226119907-1d836117d2fe.jpg" alt="Placeholder Image">
      </figure>

      <span class="whitespace-normal text-sm relative left-[.25rem] bottom-[.5rem] responsiveText">Test</span>
      <span class="flex flex-row col-start-4 relative left-[.25rem] bottom-[.5rem] whitespace-normal responsiveText">fefefe </span>
  </div>
</div>