<script>
    import darklogo from "../../routes/public/darklogo.png";
    import wave from "../../routes/public/wave.png";
    import about from "../../routes/public/about.jpg";
    import swirl from "../../routes/public/swirl.png";
</script>
<div class="">
    <div class="flex bg-white py-2 px-8 border-b-2 font-semibold  hover:cursor-pointer justify-between w-full md:text-md text-sm font-poppins">
        <div class=" hidden md:flex items-center flex">
            <div class="border-2 border-black md:px-4 px-2 bg-black text-white  hover:bg-black hover:text-white">
                <a href="/about">
                    ABOUT US
                </a>
            </div>
        </div>
        <div>
            <a href="/">
                <img src={darklogo} alt="logo" class="w-10 opacity-80">
            </a>
        </div>
        <div class="flex gap-4 items-center">
            <a href="/shop" class="border-2 border-black md:px-4 px-2 hover:bg-black hover:text-white">
                SHOP
            </a>
            <a href="/shop">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke="#000000" d="M15.75 10.5V6a3.75 3.75 0 10-7.5 0v4.5m11.356-1.993l1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 01-1.12-1.243l1.264-12A1.125 1.125 0 015.513 7.5h12.974c.576 0 1.059.435 1.119 1.007zM8.625 10.5a.375.375 0 11-.75 0 .375.375 0 01.75 0zm7.5 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z" />
                </svg>
            </a>
        </div>
    </div>

    <div class=" md:m-8 m-2 border-2 flex flex-col justify-center items-center gap-2 pb-12 rounded-xl min-h-full border-green-800 border-opacity-40">

        <div class="mx-auto flex min-h-screen-sm max-w-screen-sm md:pt-12 pt-8 ">
                <div class="flex h-full w-3/5 left-0 right-0 mx-auto items-center justify-center bg-gray-800 back">
                    <img src={about} class="object-cover " alt="about" style="border: 6px solid; border-image: linear-gradient(to bottom, #FFA500, #FFFF) 1;">
                </div>
        </div>

        <div class="md:max-w-700 mx-auto opacity-90"><span class="line-text-orange md:text-[100px] text-[75px] font-black font-poppins">ABOUT</span></div>      

        <div>
            <img src={swirl} class="absolute bottom-1 left-0 w-screen object-cover opacity-20 transform" alt="swirl">
        </div>
        
        <div class="md:w-3/4 w-5/6 left-0 right-0 mx-auto text-center font-poppins opacity-80 text-xs md:text-lg">
            At the Tote Co., we are a passionate group of students dedicated to making a <span class="font-semibold text-green-700">POSITIVE IMPACT</span> on the environment. Our mission is to provide <span class="font-semibold text-green-700">STYLISH AND SUSTAINABLE</span> tote bags that not only look good but also contribute to a greener planet. Our tote bags are made from high-quality, eco-friendly materials, ensuring durability and minimal environmental impact. We believe that small actions can lead to significant change, and choosing a sustainable tote bag is a simple yet impactful way to reduce single-use plastic and promote a more sustainable lifestyle. Whether you're a student, a professional, or someone who cares about the planet, our tote bags are designed to fit seamlessly into your daily life. <span class="font-semibold text-green-700">Join us in our journey towards a more sustainable future, one tote bag at a time!</span>
        </div>
        

        <div>
            <img src={wave} class="z-20 absolute bottom-0 left-0 w-screen object-cover opacity-10" alt="wave">
        </div>
    </div>
</div>