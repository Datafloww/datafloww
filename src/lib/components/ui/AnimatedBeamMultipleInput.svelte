<script lang="ts">
    // Scroll down to see the original Component
    import { cn } from "$lib/utils/cn.js";
    import AnimatedBeam from "$lib/components/AnimatedBeam.svelte";
    import Circle from "$lib/components/Circle.svelte";
    import { lazyLoad } from "$lib/utils/lazyLoad.js";
    import web from "$lib/assets/web.png"
    import dashboard from "$lib/assets/dashboard.png"
    import product from  "$lib/assets/product.png"
    import decision from "$lib/assets/decision.png" 
    let containerRef;
    // Circles
    let div1Ref;
    let div2Ref;
    let div3Ref;
    let div4Ref;
    let div5Ref;
    let div6Ref;
    let div7Ref;
    let className: any = "";
    let tooltips = [
    {
			name: 'User tracking',
			place: 'tooltip-left'
		},
		{
			name: 'User behaviour',
			place: 'tooltip-right'
		},
		{
			name: 'Sharper analysis',
			place: 'tooltip-right'
		},
		{
			name: 'Product insights',
			place: 'tooltip-right'
		},
		{
			name: 'Data-driven decision',
			place: 'tooltip-right'
		}]
    export { className as class };
  </script>
  
  <div
    bind:this={containerRef}
    class={cn(
      "relative flex  items-center justify-center overflow-hidden p-10 mx-6 m-auto dark:shadow-[#090909]",
      className
    )}
  >
    <!--  Gradient Line -->
    <div
      class="absolute right-5 top-0 h-px w-1/2 bg-gradient-to-l from-transparent via-white/30 via-10% to-transparent"
    />
    <!-- Main Component  -->
  
    <div
      class="flex h-full w-full flex-row justify-between gap-10 max-w-lg items-center"
    >
      <div class="flex flex-col justify-center gap-2">

        <Circle tooltip={tooltips[0].name} tooltip_place={tooltips[0].place} >
           <img  bind:this={div5Ref} src={web}  alt="" srcset="">
        </Circle>
      </div>
      <div class="flex flex-col justify-center">
        <!-- Div 6 -->
        <Circle tooltip=""  tooltip_place="" hidden={true}>
          <svg
            bind:this={div6Ref}
            xmlns="http://www.w3.org/2000/svg"
            shape-rendering="geometricPrecision"
            text-rendering="geometricPrecision"
            image-rendering="optimizeQuality"
            fill-rule="evenodd"
            clip-rule="evenodd"
            viewBox="0 0 512 512"
            >
            <svg version="1.1" id="Layer_1" xmlns:x="&amp;ns_extend;" xmlns:i="&amp;ns_ai;" xmlns:graph="&amp;ns_graphs;" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 315 99.4249573" style="enable-background:new 0 0 315 99.4249573;" xml:space="preserve">
      <style type="text/css">.st0{fill:url(#SVGID_1_);}	.st1{fill:url(#SVGID_00000142884029725686012810000004926819081512845954_);}	.st2{fill:url(#SVGID_00000176035219246226901010000000324397292818688157_);}	.st3{fill:url(#SVGID_00000044872737005649876160000015730355736842977959_);}	.st4{fill:url(#SVGID_00000178202107482993623850000018160999021847547064_);}</style>
    <metadata>
              <sfw>
                      <slices/>
            <sliceSourceBounds bottomLeftOrigin="true" height="99.4390106" width="315" x="-12.8515596" y="-161.3473358"/>
                  </sfw>
          </metadata>
    <g id="color_index_g">
              <linearGradient id="SVGID_1_" gradientUnits="userSpaceOnUse" x1="0" y1="56.6352921" x2="125.0865555" y2="56.6352921">
                      <stop offset="0" style="stop-color:#8BFFFF"/>
            <stop offset="1" style="stop-color:#2E3DFF"/>
                  </linearGradient>
        <linearGradient id="SVGID_00000102516357668109904060000011453835778067608242_" gradientUnits="userSpaceOnUse" x1="0" y1="49.6989555" x2="220.1038513" y2="49.6989555">
                      <stop offset="0" style="stop-color:#8BFFFF"/>
            <stop offset="1" style="stop-color:#2E3DFF"/>
                  </linearGradient>
        <linearGradient id="SVGID_00000083056901641160279240000012893299078749885064_" gradientUnits="userSpaceOnUse" x1="95.0389481" y1="49.7124786" x2="315" y2="49.7124786">
                      <stop offset="0" style="stop-color:#8BFFFF"/>
            <stop offset="1" style="stop-color:#2E3DFF"/>
                  </linearGradient>
        <path class="st0" d="M125.0865555,73.5401611c-4.6553497,4.6553497-9.6921997,8.7000198-14.9582367,11.9821472&#x9;&#x9;c-14.424408,9.3106995-30.9855118,13.8896561-47.5470772,13.8896561c-22.5901375,0-45.2566681-8.6750259-62.5812416-25.9232025l0,0&#x9;&#x9;l47.3938255-47.5716019c4.6553497-4.6558151,9.6926689-8.7004833,15.0350952-12.0585394&#x9;&#x9;C67.7708817,17.2166748,125.0865555,73.5401611,125.0865555,73.5401611z"/>
        <path style="fill:url(#SVGID_00000102516357668109904060000011453835778067608242_);" d="M0,73.4887619l47.3938255-47.5716019&#x9;&#x9;c4.6553497-4.6558151,9.6926689-8.7004833,15.0350952-12.0585394&#x9;&#x9;c34.1907768-21.9035263,80.1349945-17.85886,109.9755249,12.0585394l27.7802429,27.7033825l19.9191589,19.9196205&#x9;&#x9;c-17.3245697,17.2481842-39.9147034,25.8718033-62.5053101,25.8718033c-16.5610962,0-33.1222076-4.5789566-47.4702225-13.8896561&#x9;&#x9;c-5.3424225-3.2821274-10.3797455-7.3267975-15.0350952-11.9821472&#x9;&#x9;C82.2716827,60.7186203,65.4050064,54.1548309,48.3096161,54.1548309c-13.279438,0-26.558876,4.0451317-38.0831261,12.1349335"/>
        <path style="fill:url(#SVGID_00000083056901641160279240000012893299078749885064_);" d="M315,73.5364685&#x9;&#x9;c-17.26297,17.2511139-39.8813171,25.8884888-62.5116119,25.8884888c-22.6183472,0-45.2248993-8.6373749-62.4878845-25.8767014&#x9;&#x9;c-0.0118561-0.0117874-0.0118561-0.0117874-0.0118561-0.0117874&#x9;&#x9;c-22.7486572-22.7487373-58.5778809-25.8056183-84.8456039-7.2275009l-10.1040955,7.1811447l47.3077621-47.5956573&#x9;&#x9;c34.5140839-34.5259438,90.4854126-34.5259438,125.0113525,0l27.7605286,27.7605419L315,73.5364685z"/>
          </g>
    <g>
              <g>
                      <linearGradient id="SVGID_00000163052799127808498160000001101867248005661855_" gradientUnits="userSpaceOnUse" x1="100.5101547" y1="41.0018616" x2="167.6694794" y2="92.4016724">
                              <stop offset="0" style="stop-color:#000000;stop-opacity:0.5"/>
                <stop offset="1" style="stop-color:#000000;stop-opacity:0"/>
                          </linearGradient>
            <path style="fill:url(#SVGID_00000163052799127808498160000001101867248005661855_);" d="M105.1476288,66.3110428&#x9;&#x9;&#x9;c26.2523804-18.6060371,62.1036987-15.5264168,84.8490448,7.2390594c4.6594238,4.6494217,9.6987,8.6689224,15.0280914,12.0584412&#x9;&#x9;&#x9;c-5.6992188,3.6395493-11.7184601,6.5591507-17.9376373,8.7588806&#x9;&#x9;&#x9;c-9.2988434-8.8088608-10.4886322-19.8674316-29.5862732-28.3163528&#x9;&#x9;&#x9;c-22.2871552-9.8787308-60.2021942,6.4591904-62.4619064,7.4390411&#x9;&#x9;&#x9;C95.0389481,73.4901123,102.6187286,68.1033707,105.1476288,66.3110428z"/>
                  </g>
        <g>
                      <linearGradient id="SVGID_00000116229412353520279580000009624106498607554718_" gradientUnits="userSpaceOnUse" x1="5.4712067" y1="41.0018616" x2="72.6305313" y2="92.4016724">
                              <stop offset="0" style="stop-color:#000000;stop-opacity:0.5"/>
                <stop offset="1" style="stop-color:#000000;stop-opacity:0"/>
                          </linearGradient>
            <path style="fill:url(#SVGID_00000116229412353520279580000009624106498607554718_);" d="M10.1086817,66.3110428&#x9;&#x9;&#x9;c26.2523766-18.6060371,62.1037064-15.5264168,84.8490448,7.2390594c4.6594315,4.6494217,9.6987,8.6689224,15.0280914,12.0584412&#x9;&#x9;&#x9;c-5.6992188,3.6395493-11.7184601,6.5591507-17.9376297,8.7588806&#x9;&#x9;&#x9;c-9.298851-8.8088608-10.4886398-19.8674316-29.5862732-28.3163528C40.1747513,56.1723404,2.2597182,72.5102615,0,73.4901123&#x9;&#x9;&#x9;C0,73.4901123,7.5797801,68.1033707,10.1086817,66.3110428z"/>
                  </g>
          </g>
  </svg>
            </svg
          >
        </Circle>
      </div>
      <div class="flex flex-col justify-center">
        <!-- Div 7 -->
        <Circle tooltip={tooltips[1].name} tooltip_place={tooltips[1].place}>
          <svg
            bind:this={div7Ref}
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-user"
            ><path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2" /><circle
              cx="12"
              cy="7"
              r="4"
            /></svg
          >
        </Circle>

        <Circle tooltip={tooltips[2].name} tooltip_place={tooltips[2].place}>
         <img bind:this={div1Ref} use:lazyLoad={dashboard} alt="" srcset="">
        </Circle>

        <Circle tooltip={tooltips[3].name} tooltip_place={tooltips[3].place}>
          <img bind:this={div2Ref} use:lazyLoad={product} alt="" srcset="">
        </Circle>

        <Circle tooltip={tooltips[4].name} tooltip_place={tooltips[4].place}>
         <img bind:this={div3Ref} use:lazyLoad={decision} alt="" srcset="">
        </Circle>

     
      </div>
    </div>
  
    <AnimatedBeam bind:containerRef bind:fromRef={div6Ref} bind:toRef={div1Ref} />
    <AnimatedBeam bind:containerRef bind:fromRef={div6Ref} bind:toRef={div2Ref} />
    <AnimatedBeam bind:containerRef bind:fromRef={div6Ref} bind:toRef={div3Ref} />
    <!-- <AnimatedBeam bind:containerRef bind:fromRef={div6Ref} bind:toRef={div4Ref} /> -->
    <AnimatedBeam bind:containerRef bind:fromRef={div5Ref} bind:toRef={div6Ref} />
    <AnimatedBeam bind:containerRef bind:fromRef={div6Ref} bind:toRef={div7Ref} />
  </div>