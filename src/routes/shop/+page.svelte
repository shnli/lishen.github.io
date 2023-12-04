<script>
    import '../../app.css'
    import Item from '../components/item.svelte'; 
    import swirl from "../../routes/public/shopswirl.png"
    import shopwhite from "../../routes/public/shopwhite.svg"
    import circle from "../../routes/public/circle.png"
    import heart from "../../routes/public/heart.svg"
    import Marque from '../components/marque.svelte';
    import wave from "../../routes/public/wave.png"

    import coffee from "../../routes/public/inventory/coffee.jpg"
    import dino from "../../routes/public/inventory/dino.jpg"
    import kind from "../../routes/public/inventory/kind.jpg"
    import pickleball from "../../routes/public/inventory/pickleball.jpg"
    import rev from "../../routes/public/inventory/rev.jpg"
    import texas from "../../routes/public/inventory/texas.jpg"

</script>
<style>
</style>
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Finger+Paint&family=Poppins:wght@100;200;300;400;600;700;900&display=swap" rel="stylesheet">
</head>
    
<div>
    <div class="flex flex-col font-poppins md:p-8 p-2">
        <div class="bg-white fixed z-20 md:bottom-12 bottom-4 shadow-md md:w-1/3 w-5/6 left-0 right-0 mx-auto rounded-full md:text-lg text-sm border-green-800 border-2 bg-opacity-90 m-4">
            <div class="flex items-center justify-between py-2 md:px-8 px-6 md:gap-4 gap-2">
                <a href="/" class="flex flex-col justify-center items-center self-center font-semibold rounded-xl md:border-2 pt-2 border-gray-100 hover:border-green-800">
                    <img src={heart} alt="HOME" class="w-6 h-6">
                    <span class="self-center font-semibold md:px-6 px-4 ">HOME</span>
                </a>
                <a href="/shop" class="flex flex-col justify-center items-center self-center font-semibold rounded-xl border-2 pt-2 bg-gradient-to-r from-teal-700 to-green-700 opacity-90 text-white border-green-800 hover:opacity-100">
                    <img src={shopwhite} alt="SHOP" class="w-6 h-6 ">
                    <span class=" md:px-8 px-4">SHOP</span>
                </a>
                <a href="/bag" class="flex flex-col justify-center items-center self-center font-semibold rounded-xl md:border-2 pt-2 border-gray-100 hover:border-green-800">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 10.5V6a3.75 3.75 0 10-7.5 0v4.5m11.356-1.993l1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 01-1.12-1.243l1.264-12A1.125 1.125 0 015.513 7.5h12.974c.576 0 1.059.435 1.119 1.007zM8.625 10.5a.375.375 0 11-.75 0 .375.375 0 01.75 0zm7.5 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z" />
                    </svg>
                    <span class="hover:text-black font-semibold  md:px-8 px-4">BAG</span>
                </a>
            </div>
        </div>

        <div class="absolute w-full top-0 z-20 left-0 bg-black text-white">
            <Marque>
                <div class=" flex flex-col md:gap-4 gap-2 py-1">
                    <div class="md:text-md text-xs"> DISCOVER THE LATEST TOTE DESIGNS AT THE TOTE CO  •  LIMITED TIME OFFERS AVAILABLE  •  SHOP NOW  •  DISCOVER THE LATEST TOTE DESIGNS AT THE TOTE CO  •  LIMITED TIME OFFERS AVAILABLE  •  SHOP NOW  •  </div>
                </div>
            </Marque>
        </div>

        <div>
            <img src={swirl} class="absolute top-12 left-0 w-screen object-cover opacity-30" alt="swirl">
        </div>
        <div>
            <img src={swirl} class="absolute bottom-0 left-0 w-screen h-full object-cover opacity-10 transform scale-y-(-1)" alt="swirl">
        </div>
        
        <div class="shop-bg flex flex-col border-2 border-green-800 rounded-lg min-h-screen md:p-8 p-4 mt-8 border-opacity-50 justify-center align-center items-center">
            <img src={circle} class="circle" alt="GREEN BY DESIGN">
            <div class="md:max-w-700 mx-auto opacity-90 md:mb-24 mb-12"><span class="line-text-orange md:text-[100px] text-[100px] font-black">SHOP</span></div>      
            <div class="grid grid-cols-2 md:grid-cols-3 md:gap-12 gap-4 justify-center item-center text-center mb-12">
                <Item imageSrc={coffee} title="Coffee" price="$10.00" />
                <Item imageSrc={dino} title="Dinosaur" price="$10.00" />
                <Item imageSrc={kind} title="Kind Human" price="$10.00" />
                <Item imageSrc={pickleball} title="Pickleball" price="$10.00" />
                <Item imageSrc={rev} title="Reville" price="$10.00" />
                <Item imageSrc={texas} title="Texas Grown" price="$10.00" />
            </div>
        </div>


        <div class="md:mt-6 mt-4">
            <div class="flex text-gray-800 text-xs md:w-8/9 left-0 right-0 mx-auto justify-between border-opacity-60 border-gray border-2 md:border-[2px] border-green-800 opacity-60 rounded-lg md:px-12 px-4 py-8 gap-8">
                <div class="flex flex-col gap-2">
                    <div>
                        Welcome to The Tote Co! 
                    </div>
                    <div>
                        Explore our stylish collection of ecofriendly tote bags and accessories.
                    </div>
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

    </div>
    <div class= 'bottom-0 w-full translate-y-12 opacity-75'>
        <img src={wave} alt="">
    </div>
</div>
