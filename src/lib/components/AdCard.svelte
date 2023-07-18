<script>
  import ToggleButton from "./ToggleButton.svelte";
  export let image1;
  export let image2;
</script>

<style>
  figure{
    @apply text-gray-two;
  }
</style>

<div class="grid col-span-1 bg-white-one w-[100%] h-[100%] p-2 rounded-lg">
  <span class="justify-end grid grid-cols-2 text-purple-one font-semibold p-2">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-5 h-5">
      <defs>
        <filter id="glow-effect" x="-20%" y="-20%" width="140%" height="140%">
          <feGaussianBlur in="SourceGraphic" stdDeviation="2" result="blur" />
          <feFlood flood-color="#5650e3" result="color" />
          <feComposite in="color" in2="blur" operator="in" result="glow" />
          <feMerge>
            <feMergeNode in="glow" />
            <feMergeNode in="SourceGraphic" />
          </feMerge>
        </filter>
      </defs>
      <g filter="url(#glow-effect)">
        <path fill="#5650e3" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" d="M12 0c6.623 0 12 5.377 12 12s-5.377 12-12 12-12-5.377-12-12 5.377-12 12-12zm0 1c6.071 0 11 4.929 11 11s-4.929 11-11 11-11-4.929-11-11 4.929-11 11-11zm0 11h6v1h-7v-9h1v8z" />
      </g>
    </svg>
    
    <div class="flex flex-row justify-end flex-shrink-0">
      <span class="pr-4">edit</span>
      <ToggleButton />
    </div>
  </span>

    <div class="grid grid-cols-5 gap-2 w-[100%] h-[100%] pb-[.5rem]">
      <figure class='grid col-span-3'>
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class="rounded-lg w-full h-full object-cover aspect-square" src="{image1}" alt="Placeholder Image">
      </figure>

      <figure class='grid col-span-2'>
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class="rounded-lg object-cover w-full h-full" src="{image2}" alt="Placeholder Image">
      </figure>

      <span class="whitespace-normal text-sm relative left-[.25rem] bottom-[.5rem] responsiveText">Test</span>
      <span class="flex flex-row col-start-4 relative left-[.25rem] bottom-[.5rem] whitespace-normal responsiveText">fefefe </span>
  </div>
</div>