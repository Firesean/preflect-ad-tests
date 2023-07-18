<script>
    export let svgPathing;
    export let label;
    export let link;
    export let rotation;
  </script>
  
  <a href="{link}" class="text-gray-700 hover:text-indigo-600 hover:bg-gray-50 group flex gap-x-3 rounded-md text-sm leading-6 font-semibold h-[1.5rem] w-[10rem]">
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6" style="transform: rotate({rotation}deg);">
      <path stroke-linecap="round" stroke-linejoin="round" d="{svgPathing}" />
    </svg>
    <span class="responsiveText hidden sm:block">{label}</span>
  </a>
  