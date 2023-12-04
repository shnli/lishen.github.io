<script>
    import landingJpg from "../routes/public/landing.jpg"
    import logoWhite from "../routes/public/logo.png"
    import cornerBottomRight from "../routes/public/corner-bottom-right.svg"
    import cornerTopLeft from "../routes/public/corner-top-left.svg"
    import cornerBottomLeft from "../routes/public/corner-bottom-left.svg"
    import cornerTopRight from "../routes/public/corner-top-right.svg"
    import wave from "../routes/public/wave.png"
    import '../app.css'
    import Item from './components/newitem.svelte';
    import whiteheart from "../routes/public/whiteheart.svg"
    import shop from "../routes/public/shop.svg"
    import Marque from './components/marque.svelte';
    import darklogo from "../routes/public/darklogo.png"
    import coffee from "../routes/public/inventory/coffee.jpg"
    import dino from "../routes/public/inventory/dino.jpg"
    import rev from "../routes/public/inventory/rev.jpg"


    let scrolledToNewItems = false;

    function handleScroll() {
        const newItemsSection = document.getElementById('newItemsSection');

        if (newItemsSection) {
            const newItemsPosition = newItemsSection.getBoundingClientRect().top;

            scrolledToNewItems = window.scrollY > newItemsPosition;
        }
    }

    

</script>

<style>
    .fixed-navbar {
        transition: transform 0.3s ease-in-out;
        transform: translateY(-100%);
    }

    .fixed-navbar.visible {
        transform: translateY(0);
    }
</style>


<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Finger+Paint&family=Poppins:wght@100;200;300;400;600;700;900&display=swap" rel="stylesheet">
</head>
    
<div class="flex flex-col font-poppins" on:scroll={handleScroll}>

    <div class="absolute w-full top-0 z-20 left-0 bg-black text-white">
        <Marque>
            <div class=" flex flex-col md:gap-4 gap-2 py-1">
                <div class="md:text-md text-xs"> DISCOVER THE LATEST TOTE DESIGNS AT THE TOTE CO  •  LIMITED TIME OFFERS AVAILABLE  •  SHOP NOW  •  DISCOVER THE LATEST TOTE DESIGNS AT THE TOTE CO  •  LIMITED TIME OFFERS AVAILABLE  •  SHOP NOW  •  </div>
            </div>
        </Marque>
    </div>



    <div class="bg-white fixed z-20 md:bottom-12 bottom-4 shadow-md md:w-1/3 w-5/6 left-0 right-0 mx-auto rounded-full md:text-lg text-sm border-green-800 border-2 bg-opacity-90 m-4">     
            <div class="flex items-center justify-between py-2 md:px-8 px-6 md:gap-4 gap-2">
            <a href="/" class="flex flex-col justify-center items-center self-center font-semibold rounded-xl md:border-2 pt-2 bg-gradient-to-r from-teal-700 to-green-700 opacity-90 text-white border-green-800 hover:opacity-100">
                <img src={whiteheart} alt="SHOP" class="w-6 h-6">
                <span class="self-center font-semibold md:px-6 px-4 ">HOME</span>
            </a>
            <a href="/shop" class="flex flex-col justify-center items-center self-center font-semibold rounded-xl border-2 pt-2 border-gray-100 hover:border-opacity-100 hover:border-green-800">
                <img src={shop} alt="shop" class="w-6 h-6 ">
                <span class=" md:px-8 px-4">SHOP</span>
            </a>
            <a href="/bag" class="flex flex-col justify-center items-center self-center font-semibold rounded-xl md:border-2 pt-2 border-gray-100 hover:border-opacity-100 hover:border-green-800">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 10.5V6a3.75 3.75 0 10-7.5 0v4.5m11.356-1.993l1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 01-1.12-1.243l1.264-12A1.125 1.125 0 015.513 7.5h12.974c.576 0 1.059.435 1.119 1.007zM8.625 10.5a.375.375 0 11-.75 0 .375.375 0 01.75 0zm7.5 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z" />
                </svg>
                <span class="hover:text-black font-semibold md:px-8 px-4">BAG</span>
            </a>
        </div>
    </div>

      
        <div class="flex bg-white z-10 md:mt-6 mt-4 py-2 px-8 font-semibold hover:cursor-pointer justify-between w-full md:text-md text-sm">
            <div class="border-2 border-black md:px-4 px-2  hover:bg-black hover:text-white">
                <a href="/about">
                    ABOUT US
                </a>
            </div>
            <div class="flex gap-4 items-center">
                <a href="/shop" class="border-2 border-black md:px-4 px-2  hover:bg-black hover:text-white">
                    SHOP
                </a>
                <a href="/shop">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke="#000000" d="M15.75 10.5V6a3.75 3.75 0 10-7.5 0v4.5m11.356-1.993l1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 01-1.12-1.243l1.264-12A1.125 1.125 0 015.513 7.5h12.974c.576 0 1.059.435 1.119 1.007zM8.625 10.5a.375.375 0 11-.75 0 .375.375 0 01.75 0zm7.5 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z" />
                    </svg>
                </a>
            </div>
        </div>

        <div class="background-image flex flex-col bg-black pt-36 pb-24 md:pb-36 ">
            <div class="flex md:left-8 left-1 md:top-8 top-1 absolute">
                <img src={cornerTopLeft} width="72" class="opacity-50" alt="corner">
            </div>
            <div class="flex md:right-8 right-1 md:bottom-8 bottom-1 absolute">
                <img src={cornerBottomRight} width="72" class="opacity-50" alt="corner">
            </div>
            <div class="flex md:left-8 left-1 md:bottom-8 bottom-1 absolute">
                <img src={cornerBottomLeft} width="72" class="opacity-50" alt="corner">
            </div>
            <div class="flex md:right-8 right-1 md:top-8 top-1 absolute">
                <img src={cornerTopRight} width="72" class="opacity-50" alt="corner">
        </div>
        <div class="flex w-full justify-center items-center absolute top-6">
            <img src={logoWhite} width="64" class="opacity-90" alt="The Tote Co. Logo">
        </div>
        <div class="flex image-content md:px-24 px-8 min-h-[200px]">
            <div class="absolute md:left-24 left-4 right-4 mx-auto md:top-36 top-28 md:text-[200px] text-[75px] font-black md:text-start text-center" style="line-height: 1;">
                <h1 class="md:max-w-700  md:text-start mx-auto opacity-90">
                    <span class="line-text md:text-[200px] text-[60px]">GREEN BY</span>  <span class="text-image-clip font-fp">DESIGN.</span>
                </h1>
            </div>
            <div class="md:w-96 md:h-96 mt-20 md:mt-0 rounded-xl flex " style="border: 5px solid rgba(255, 255, 255, 0.221); overflow: hidden;">
                <img src="{landingJpg}" alt="pickleball bag" style="object-fit: cover; " class="">
            </div>
        </div>
    </div>

    <hr class="mb-8 border-[3px] border-green-800">

    <div class="flex flex-col justify-top items-center bg-white bg-image-orange-vector">
        <p class="title">
            NEW ARRIVALS
        </p>
        <hr class="border-2 border-orange-300 w-12 mb-8 mt-4">
        <div class="grid md:grid-cols-3 grid-cols-1 gap-12 justify-center item-center text-center mb-12">
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
            <Item imageSrc={dino} title="Dinosaur Bag" price="$10.00" />
            <Item imageSrc={rev} title="Pickleball Bag" price="$10.00" />
        </div>
    </div>
    
    <div class="md:mt-16 mt-8 px-8">
        <div class="flex text-gray-800 text-xs md:w-8/9 left-0 right-0 mx-auto justify-between border-opacity-60 border-gray border-2 md:border-[2px] border-green-800 opacity-60 rounded-lg md:px-12 px-4 py-8 gap-8">
            <div class="flex flex-col gap-4 justify-center items-center">
                <div class="flex flex-col gap-2 text-start">
                    <div class="">
                        Welcome to The Tote Co! 
                    </div>
                    <div>
                        Explore our stylish collection of ecofriendly tote bags and accessories.
                    </div>
                </div>
                <img src="{darklogo}" alt="logo" class="md:w-24 w-12 items-center opacity-40">
            </div>
            <div class="flex flex-col gap-2">
                <div>
                    Contact us at: <a href="mailto:info@thetoteco.com" class="text-green-800">info@thetoteco.com</a>
                </div>
                <div>
                    Connect with us on social media: <a href="https://www.instagram.com/TheToteCo" target="_blank" class="text-green-800">@TheToteCo</a> | <a href="https://www.twitter.com/TheToteCo" target="_blank" class="text-green-800">@TheToteCo</a>
                </div>
                <div>
                    Visit our store at: 1234 Tote Street, EcoCity, Earth
                </div>
            </div>
        </div>
    </div>
   
    <div class= 'bottom-0 w-full md:translate-y-12 translate-y-24 opacity-75'>
        <img src={wave} alt="wave">
    </div>
</div>
