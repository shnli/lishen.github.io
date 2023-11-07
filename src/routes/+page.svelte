<style>
    .first-section {
        position: relative; /* Add this to make the overlay positioning relative to the parent element */
        background-image: url('./bg.png');
        background-size: cover; 
        background-repeat: no-repeat;
    }

    .first-section::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        /* background-color: rgba(0, 0, 0, 0.3); */
    }
</style>

<div class="flex flex-col">
    <div class="first-section flex flex-col justify-top items-end h-screen bg-green-800 p-24 justify-between">
        <div class="absolute left-24 top-24 text-[135px] font-black text-start text-white" style="line-height: 1;">
            <div>GREEN BY</div>
            <div>DESIGN</div>
        </div>
    
        <div class="w-96 h-96 bg-gray-500 rounded-xl">
        </div>
    </div>
    <div class="align-bottom">
        <div class="flex justify-between w-96 bg-white px-8 py-2 rounded-lg ">
            <p>ABOUT US</p>
            <p>SHOP</p>
        </div>
    </div>
    <div class="flex flex-col justify-top items-center h-screen bg-white p-24 gap-8">
        <p class="font-bold">
            NEW ARRIVALS
        </p>
        <div class="flex justify-between w-full">
            <div class="w-72 h-96 bg-gray-200 rounded-xl">
            </div>
            <div class="w-72 h-96 bg-gray-200 rounded-xl">
            </div>
            <div class="w-72 h-96 bg-gray-200 rounded-xl">
            </div>
            <!-- <img src='./placeholder.jpg' alt="...">
            <img src='./placeholder.jpg' alt="..."> -->
        </div>
    </div>
</div>
