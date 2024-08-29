<script>
    import logo from '$lib/assets/logo.svg';
    import DotBackground from '$lib/components/ui/DotBackground.svelte';
    import dashboard from "$lib/assets/dashboard.avif";
    import github from "$lib/assets/github.svg";
    import msfs from "$lib/assets/dataflow_ms.jpg";
    import mail from "$lib/assets/mail.png";
    import AnimatedBeamMultipleInput from '$lib/components/ui/AnimatedBeamMultipleInput.svelte';
    import Team from '../lib/components/Team.svelte';
    import Card from '../lib/components/Card.svelte';
    import { lazyLoad } from '$lib/utils/lazyLoad';
</script>
 


<div class="navbar navbar-scroll backdrop-filter bg-slate-300 backdrop-blur-lg bg-opacity-40 border-b border-gray-200 z-20">
        <div class="navbar-start">
            <div class="dropdown">    
        <div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
          <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor">
          <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h8m-8 6h16" />
          </svg>
        </div>
        <ul
        tabindex="-1"
        class="menu menu-sm dropdown-content bg-white rounded-box z-[1] mt-3 w-52 p-2 shadow">
        <li class="text-lg"><a href="/">Login</a></li>
        <li class="text-lg"><a href="/">Home</a></li>
        <li class="text-lg"><a href="#features">Features</a></li>
    </ul>
</div>
<img src={logo} alt="datafloww logo" class="mx-2" width="64">
<p class="text-xl hidden lg:flex font-bold px-2">Datafloww</p>
</div>
<div class="navbar-center hidden lg:flex">
    <ul class="menu menu-horizontal px-1">
        <li class="text-lg px-6"><a href="/">Home</a></li>
        <li class="text-lg"><a href="#features">Features</a></li>
    </ul>
</div>
<div class="navbar-end">
    <button class=" lg:flex lg:py-3 lg:px-7 lg:rounded-full lg:border-x lg:border-y hidden lg:text-blue-600 lg:border-blue-500 lg:hover:bg-slate-300 ">Login</button>
    <button class="btn rounded-full bg-blue-500 border-none m-2 lg:mx-4 text-white hover:bg-blue-700">Get started</button>
</div>
</div>

<div class="hero z-10"> 
        <DotBackground >
        <div class="hero-content text-center animate-slidein300">
            <div class="max-w-2xl">
                <h1 class="lg:text-4xl md:text-3xl text-2xl lg:font-bold font-semibold leading-tight lg:leading-snug">Elevate your business <span class="bg-gradient-to-r text-transparent from-[#3546ff] via-[#5aa6f8] to-blue-700 bg-clip-text">flow</span> with sharper analytics and product insights.</h1>
                <p class="py-5 lg:text-lg text-md font-medium bg-slate-100 w-fit h-16 px-1 bg-opacity-80 rounded-xl m-auto">
                    Unlock growth with data-driven decisions and actionable insights.
                </p>
                <button disabled class="bg-blue-500 w-fit text-lg md:text-sm md:p-3 lg:text-base m-auto p-3 mt-10 lg:mt-2 hover:shadow-blue-400 rounded-full duration-300 text-white hover:px-4 hover:duration-300 hover:shadow-xl animate-slidein500">Coming soon</button>
            </div>
        </div>
    </DotBackground>
</div>    

<div class="lg:h-[30.4rem] md:h-[22rem] h-40 relative w-full overflow-hidden bg-slate-50 animate-slidein700">
    <img src={dashboard} alt="" class="lg:px-28 px-3"></div>
<div class=" pt-20 bg-slate-100">
    <h1 class="text-center font-semibold text-2xl lg:text-5xl">Get every <span class="bg-gradient-to-r text-transparent from-[rgb(53,70,255)] via-[#5aa6f8] to-blue-700 bg-clip-text">insight</span> at one place!</h1>
    <AnimatedBeamMultipleInput />
</div>


<div class="bg-dot-black/[0.4] py-8 ">
    <h1 class="text-center font-semibold text-3xl lg:text-4xl mb-6 " id="features">Features</h1>
    <div class="w-full grid lg:grid-cols-2 grid-cols-1 gap-y-8 ">
        <Card />
    </div>
</div>


<div class="w-full bg-gradient-to-b from-slate-50 to-slate-100 flex justify-center px-5 lg:px-44 py-10 lg:py-20 mb-5">
    <img src={msfs} class="drop-shadow-lg" alt="">
</div>


<h1 class="text-center font-semibold text-3xl m-auto p-4">Our <span class="bg-gradient-to-r text-transparent from-[#3546ff] via-[#5aa6f8] to-blue-700 bg-clip-text">Team</span></h1>
<div class="grid grid-cols-4 py-4 mb-20">
   <Team/>
</div>

<div class="grid grid-cols-2 bg-slate-100 text-center text-lg border-2 border-t-gray-300 ">
    <a href="https://mail.google.com/mail/u/0/?view=cm&fs=1&tf=1&source=mailto&to=datafloww.in@gmail.com">
        <div class="flex flex-col items-center w-fit m-auto p-4 rounded-xl cursor-pointer hover:bg-slate-200">
            <img use:lazyLoad={mail} class="w-6" alt="">
            <div>Mail</div>
        </div>
    </a>

    <a href="https://github.com/DataFloww">
        <div class="flex flex-col items-center w-fit m-auto p-4 duration-200 rounded-xl cursor-pointer hover:bg-slate-200">
            <img use:lazyLoad={github} alt="">
            <div>Github</div>
        </div>
    </a>
</div>
