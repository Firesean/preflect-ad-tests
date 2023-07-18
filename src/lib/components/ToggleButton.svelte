<script>
    let isChecked = false;
  
    function toggleSwitch() {
      isChecked = !isChecked;
    }
  </script>
  
  <!-- svelte-ignore a11y-no-static-element-interactions -->
  <!-- svelte-ignore a11y-click-events-have-key-events -->
  <div class="h-[1.5rem] w-[3rem] rounded-full {isChecked ? 'bg-purple-one' : 'bg-gray-three'}" on:click={toggleSwitch}>
    <div class="h-[1.25rem] w-[1.25rem] m-[.125rem] rounded-full bg-white-one {isChecked ? 'translate-x-[1.5rem] duration-300' : 'translate-x-0 duration-300'}"></div>
  </div>
  