<script lang="ts">
	export let tooltip:string;
	export let tooltip_place:string;
	export let hidden = false;
  </script>
  
  <div
    class={
      `z-10 flex h-12 w-12 lg:h-[4.2rem] lg:w-[4.2rem] items-center bg-slate-100 justify-center rounded-full border-2 dark:bg-background p-3 mb-8 shadow-[0_0_20px_-12px_rgba(0,0,0,0.8)] hover:border-blue-500 hover:shadow-xl dark:hover:border-cyan-300 dark:hover:bg-[#051a22] transition-all duration-200 cursor-pointer ${hidden?"":`tooltip lg-${tooltip_place} md-${tooltip_place}`} tooltip-bottom`	
	}
	data-tip={tooltip}
  >
    <slot></slot>
  </div>
  