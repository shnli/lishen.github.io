
<script>
    export let imageSrc;
    export let title;
    export let price;
  </script>
  
  <div class="flex flex-col gap-4 border-2 shadow-md w-1/5 p-4 rounded-xl">
    <img src={imageSrc} alt="Coffee" class="rounded-xl h-[300px] mx-auto">
    <div>
      <div>{title}</div>
      <div>{price}</div>
    </div>
  </div>