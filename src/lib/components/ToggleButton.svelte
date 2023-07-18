<script>
    let isChecked = false;
  
    function toggleSwitch() {
      isChecked = !isChecked;
    }
</script>

<label class="items-center cursor-pointer">
    <div class="relative">
      <input type="checkbox" class="hidden" bind:checked={isChecked} />
      <div class="w-10 h-4 bg-red-400 rounded-full shadow-inner"></div>
      <div class="dot absolute w-6 h-6 rounded-full shadow -left-1 -top-1 transition-transform duration-300 ease-in-out transform translate-x-0 bg-red-500" 
           class:translate-x-6={isChecked}
           class:bg-purple-600={isChecked}
      >
    </div>
    </div>
  </label>