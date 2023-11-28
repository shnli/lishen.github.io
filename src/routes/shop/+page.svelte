<script>
    import '../../app.css'
    import coffee from "../../routes/public/inventory/coffee.jpg"
    import Item from '../components/item.svelte'; // Adjust the path based on your project structure
    import swirl from "../../routes/public/shopswirl.png"
</script>
<style>
</style>
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Finger+Paint&family=Poppins:wght@100;200;300;400;600;700;900&display=swap" rel="stylesheet">
</head>
    
<div class="bg-image-orange-vectorflex flex-col font-poppins md:p-8 p-4">
    <nav class="bg-white fixed z-20 bottom-12 left-0 right-0 shadow-md md:mx-24 mx-8 rounded-xl md:text-lg text-sm border-green-800 border-[3px]">
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
    </nav>

    <!-- <div>
        <Navbar></Navbar>
    </div> -->

    <div>
        <img src={swirl} class="absolute top-12 left-0 w-screen object-cover opacity-30">
    </div>
    <div class="shop-bg flex flex-col border-2 border-green-800 rounded-lg min-h-screen p-8 border-opacity-50 justify-center align-center items-center">
        <div class="md:max-w-700 mx-auto opacity-90 mb-24"><span class="line-text-orange md:text-[100px] text-[100px] font-black">SHOP</span></div>      
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-12 justify-center item-center text-center mb-12">
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
            
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
            <Item imageSrc={coffee} title="Coffee Bag" price="$10.00" />
        </div>
    </div>

    <div class="md:mt-6 mt-1 mb-24">
        <div class="flex text-gray-400 text-xs justify-between border-gray border-2 md:border-[2px] rounded-lg px-8 py-4">
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

</div>
