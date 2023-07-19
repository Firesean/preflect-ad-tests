<script>
  import ToggleButton from "./ToggleButton.svelte";
  export let feedImg;
  export let storyImg;
</script>

<style>
  figure{
    @apply text-gray-two;
  }

  img{
    @apply rounded-lg object-cover w-full h-full;
  }

  .captionText{
    @apply whitespace-normal relative left-[.25rem] bottom-[.5rem];
  }
</style>

<!-- Clock SVG -->
<div class="grid col-span-1 bg-white-one w-[100%] h-[100%] p-2 rounded-lg min-w-[135px]">
  <span class="justify-end grid grid-cols-2 text-purple-one font-semibold p-1">
    <div class="relative flex items-center justify-center w-[1.5rem] h-[1.5rem] rounded-full bg-blue-one bg-opacity-95">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" class="w-[.9rem] h-[.9rem]">
        <path fill="#5650e3" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" d="M12 0c6.623 0 12 5.377 12 12s-5.377 12-12 12-12-5.377-12-12 5.377-12 12-12zm0 1c6.071 0 11 4.929 11 11s-4.929 11-11 11-11-4.929-11-11 4.929-11 11-11zm0 11h6v1h-7v-9h1v8z" />
      </svg>
    </div>
  
    <div class="flex flex-row justify-end flex-shrink-0">
      <span class="pr-2">edit</span>
      <ToggleButton />
    </div>
  </span>
  

    <div class="grid grid-cols-5 gap-2 w-[100%] h-[100%] pb-[.5rem]">
      <figure class='grid col-span-3'>
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img class="aspect-square" src="{feedImg}" alt="Placeholder Image">
      </figure>

      <figure class='grid col-span-2'>
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img src="{storyImg}" style="object-fit: contain" class="bg-gray-three" alt="Placeholder Image">
      </figure>

      <span class="captionText responsiveText text-gray-two">Feed</span>
      <span class="flex flex-row col-start-4 captionText responsiveText text-gray-two">Story</span>
  </div>
</div>