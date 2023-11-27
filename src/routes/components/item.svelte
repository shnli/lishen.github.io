
<script>
    export let imageSrc;
    export let title;
    export let price;
  </script>
  
  <div class="flex flex-col gap-4 border-[2px] bg-white border-green-800 shadow-md  p-8 rounded-xl">
    <img src={imageSrc} alt="Coffee" class="rounded-xl h-[300px] object-cover">
    <div>
      <div>{title}</div>
      <div>{price}</div>
    </div>
  </div>