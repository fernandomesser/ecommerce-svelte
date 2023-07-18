<script>
    /**
   * @type {{ name: string; price: number; imageUrl: string; description: string; paymentUrl: string; }}
   */
     export let product;
</script>

<div class="border-black bg-neutral-200 border rounded px-8 py-10 space-y-6 shadow">
    <h3 class="sm: text-2xl font-bold text-gray-900 sm:text-3xl">{product.name}</h3>
    <p class="mt-8 flow-root sm:mt-12">{product.description}</p>
    <div>
        <img src={product.imageUrl} class="w-full rounded-lg" />
    </div>
    <h4 class="text-3xl font-bold">${product.price}</h4>
    <div>
        <a href={product.paymentUrl} class="inline-flex items-center justify-center rounded-md border-2 border-transparent bg-gray-900 bg-none px-16 py-6 text-center text-base font-bold text-white transition-all duration-200 ease-in-out focus:shadow hover:bg-gray-800">Buy Now</a>
    </div>
</div>