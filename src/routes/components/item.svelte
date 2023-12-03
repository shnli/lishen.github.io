
<script>
    export let imageSrc;
    export let title;
    export let price;
    import addtobag from "../../routes/public/addtobag.svg"
  </script>
  
  <div class="flex flex-col gap-4 border-[2px] bg-white border-green-800 shadow-md md:p-8 p-2 rounded-xl hover:cursor-pointer md:text-md text-xs">
    <img src={imageSrc} alt="product image" class="rounded-xl h-[200px] md:h-[300px] object-cover">
    <div class="flex justify-between items-center align-center">
      <div class="text-start">
        <div class="font-semibold">{title}</div>
        <div>{price}</div>
      </div>
      <div>
        <button class="bg-gradient-to-r from-teal-600 to-green-700 border-[1px] border-green-800 text-white rounded-xl p-2">
          <img src={addtobag} alt="add to bag" class="md:w-6 md:h-6 w-4 h-4">
        </button>
        
      </div>
    </div>
  </div>