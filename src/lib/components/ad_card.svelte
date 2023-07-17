<script>
  let isChecked = false;

  function toggleSwitch() {
    isChecked = !isChecked;
  }
</script>

<div class="flex bg-white-one w-[90%] h-[90%] p-1 m-auto rounded">
    <svg xmlns="http://www.w3.org/2000/svg" fill="#5650e3" viewBox="0 0 24 24" stroke-width="1.5" stroke="white" class="w-6 h-6">
        <path stroke-linecap="round" stroke-linejoin="round" d="M12 6v6h4.5m4.5 0a9 9 0 11-18 0 9 9 0 0118 0z" /> <!-- 3 o'clock SVG, issue with the SVG stroke -->
      </svg>
      
    <span class="justify-end">edit     
      <label class="flex items-center cursor-pointer">
      <div class="relative">
        <input type="checkbox" class="hidden" bind:checked={isChecked} />
        <div class="w-10 h-4 bg-gray-400 rounded-full shadow-inner"></div>
        <div class="dot absolute w-6 h-6 rounded-full shadow -left-1 -top-1 transition-transform duration-300 ease-in-out transform translate-x-0 bg-gray-500" 
             class:translate-x-6={isChecked}
             class:bg-purple-600={isChecked}
        >
      </div>
      </div>
    </label>
  </span>

    <div class="grid grid-cols-2">
    <figure>
      <img src="../../../src/images/photo-1685226119907-1d836117d2fe.jpg" alt="Placeholder Image">
      <figcaption>Feed</figcaption>
    </figure>

    <figure>
      <img src="../../../src/images/photo-1685226119907-1d836117d2fe.jpg" alt="Placeholder Image">
      <figcaption>Story</figcaption>
    </figure>
  </div>


</div>