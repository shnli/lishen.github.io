<script>
    import coffee from "../routes/public/inventory/coffee.jpg"
    import landingJpg from "../routes/public/landing.jpg"
    import logoWhite from "../routes/public/logo.png"
    import cornerBottomRight from "../routes/public/corner-bottom-right.svg"
    import cornerTopLeft from "../routes/public/corner-top-left.svg"
    import cornerBottomLeft from "../routes/public/corner-bottom-left.svg"
    import cornerTopRight from "../routes/public/corner-top-right.svg"
    import wave from "../routes/public/wave.png"
    import '../app.css'
    import Navbar from './components/navbar.svelte'; // Adjust the path based on your project structure

</script>
<style>
</style>
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Finger+Paint&family=Poppins:wght@100;200;300;400;600;700;900&display=swap" rel="stylesheet">
</head>
    
<div class="flex flex-col font-poppins">

    <!-- <nav class="bg-white fixed z-20 bottom-12 left-0 right-0 shadow-md md:mx-24 mx-8 rounded-xl md:text-lg text-sm border-green-800 border-2">
        <div class=" flex items-center justify-between w-full mx-auto py-1 md:px-12 px-4">
            <a href="/" class="flex items-center">
                <span class="self-center font-semibold">ABOUT</span>
            </a>
            <a href="/shop" class="flex items-center">
                <span class="self-center font-semibold bg-green-800 rounded-full border-2 border-green-800 hover:border-green-800 hover:bg-white hover:text-black md:px-24 px-4 py-2 text-white">SHOP</span>
            </a>
            <a href="/" class="flex items-center md:pl-20 pl-6">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 10.5V6a3.75 3.75 0 10-7.5 0v4.5m11.356-1.993l1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 01-1.12-1.243l1.264-12A1.125 1.125 0 015.513 7.5h12.974c.576 0 1.059.435 1.119 1.007zM8.625 10.5a.375.375 0 11-.75 0 .375.375 0 01.75 0zm7.5 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z" />
                </svg>
            </a>
        </div>
    </nav> -->

    <div class="flex justify-center items-center align-center">
        <Navbar></Navbar>
    </div>
  
    <div class="background-image flex flex-col bg-black pt-36 pb-24 md:pb-36">
        <div class="flex md:left-8 left-1 md:top-8 top-1 absolute">
            <img src={cornerTopLeft} width="72" class="opacity-50">
        </div>
        <div class="flex md:right-8 right-1 md:bottom-8 bottom-1 absolute">
            <img src={cornerBottomRight} width="72" class="opacity-50">
        </div>
        <div class="flex md:left-8 left-1 md:bottom-8 bottom-1 absolute">
            <img src={cornerBottomLeft} width="72" class="opacity-50">
        </div>
        <div class="flex md:right-8 right-1 md:top-8 top-1 absolute">
            <img src={cornerTopRight} width="72" class="opacity-50">
        </div>
        <div class="flex w-full justify-center items-center absolute top-8">
            <img src={logoWhite} width="64" class="opacity-90">
        </div>
        <div class="flex image-content md:px-24 px-8 min-h-[200px]">
            <div class="absolute md:left-24 left-4 right-4 mx-auto md:top-36 top-28 md:text-[200px] text-[75px] font-black md:text-start text-center" style="line-height: 1;">
                <h1 class="md:max-w-700  md:text-start mx-auto opacity-90">
                    <span class="line-text md:text-[200px] text-[60px]">GREEN BY</span>  <span class="text-image-clip font-fp">DESIGN.</span>
                </h1>
            </div>
            <div class="md:w-96 md:h-96 mt-20 md:mt-0 rounded-xl flex " style="border: 5px solid rgba(255, 255, 255, 0.221); overflow: hidden;">
                <img src="{landingJpg}" alt="..." style="object-fit: cover; width: 100%; height: 100%;" class="">
            </div>
        </div>
    </div>

    <hr class="mb-8 border-[3px] border-green-800">

    <div class="flex flex-col justify-top items-center bg-white bg-image-orange-vector">
        <p class="title">
            NEW ARRIVALS
        </p>
        <hr class="border-2 border-orange-300 w-12 mb-8 mt-4">
        <div class="flex md:flex-row flex-col align-center items-center gap-8 justify-center w-full px-12">
            <img src='{coffee}' alt="..." class="md:w-1/5 rounded-xl">
            <img src='{coffee}' alt="..." class="md:w-1/5 rounded-xl">
            <img src='{coffee}' alt="..." class="md:w-1/5 rounded-xl">
        </div>
        
    </div>

    <div class="md:mt-16 mt-12  md:px-24 px-8">
        <div class="flex text-gray-400 text-xs justify-between border-gray border-2 md:border-[2px] rounded-full px-8 py-4">
            <div class="">
                HELLO
            </div>
            <div class="">
                <div>
                    TheToteCo@tote.com
                </div>
                <div>
                    @TheToteCo
                </div>
            </div>
        </div>
    </div>
   
    <div class= 'bottom-0 w-screen translate-y-24 opacity-75'>
        <img src={wave} alt="">
    </div>
</div>
