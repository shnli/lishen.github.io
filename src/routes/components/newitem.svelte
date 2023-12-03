
<script>
    export let imageSrc;
    export let title;
    export let price;
  </script>
  
  <div class="flex flex-col gap-4 border-[2px] bg-white border-orange-400 shadow-md p-6 rounded-xl hover:cursor-pointer md:text-md text-xs">
    <img src={imageSrc} alt="product image" class="rounded-xl w-[200px] md:w-[300px] md:h-[400px] object-cover">
    <div class="md:text-start text-center flex md:flex-row flex-col md:justify-between items-center gap-4">
      <div>
        <div class="font-semibold text-lg">{title}</div>
        <div>{price}</div>
      </div>
      <div>
        <button class=" border-2 hover:bg-orange-300 hover:text-black rounded-full py-1 px-4 border-black bg-black text-white">
          LEARN MORE
        </button>
      </div>
    </div>
  </div>