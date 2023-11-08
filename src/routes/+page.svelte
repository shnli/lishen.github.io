<script>
    import coffee from "../routes/public/inventory/coffee.jpg"
    import landingJpg from "../routes/public/landing.jpg"
    import '../app.css'
</script>
<style></style>
    
<div class="flex flex-col gap-8 font-poppins">

    <nav class="bg-white fixed z-20 bottom-12 left-0 right-0 shadow-md mx-24 rounded-xl border-[1px] border-gray-300">
        <div class=" flex flex-wrap items-center justify-between w-full mx-auto py-2 px-12">
            <a href="/" class="flex items-center">
                <span class="self-center text-lg font-semibold">ABOUT US</span>
            </a>
            <a href="/" class="flex items-center">
                <span class="self-center text-lg font-semibold">SHOP</span>
            </a>
            <a href="/" class="flex items-center">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 10.5V6a3.75 3.75 0 10-7.5 0v4.5m11.356-1.993l1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 01-1.12-1.243l1.264-12A1.125 1.125 0 015.513 7.5h12.974c.576 0 1.059.435 1.119 1.007zM8.625 10.5a.375.375 0 11-.75 0 .375.375 0 01.75 0zm7.5 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z" />
                </svg>
            </a>
        </div>
    </nav>
  
    <div class="background-image first-section flex flex-col justify-center align-center items-end bg-green-800 px-24 py-36 justify-between">
        <div class="image-content ">
            <div class=" absolute left-24 top-36 text-[200px] font-black text-start text-white" style="line-height: 1;">
                <h1 class="max-w-700"><span class="line-text">GREEN BY</span> DESIGN</h1>
            </div>
        
            <div class="w-96 h-96 rounded-xl image-content" style="overflow: hidden;">
                <img src="{landingJpg}" alt="..." style="object-fit: cover; width: 100%; height: 100%;">
            </div>
        </div>
    </div>

    <div class="flex flex-col justify-top items-center h-screen bg-white gap-8">
        <p class="title">
            NEW ARRIVALS
        </p>
        <div class="flex gap-8 justify-center w-full">
            <img src='{coffee}' alt="..." class="w-1/5 rounded-xl">
            <img src='{coffee}' alt="..." class="w-1/5 rounded-xl">
            <img src='{coffee}' alt="..." class="w-1/5 rounded-xl">
        </div>
    </div>

</div>
