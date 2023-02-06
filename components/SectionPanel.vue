<script setup>
let props = defineProps({
    title: String
})
</script>

<template>
    <div class="mx-auto max-w-2xl  sm:px-4  lg:max-w-7xl ">
        <div class="flex items-center space-x-4">
            <slot name="icon" />
            <h2 class="text-xl font-bold text-gray-900">
                {{ props.title }}
            </h2>
            <slot name="action" />
        </div>
        <div class="mt-3 grid grid-cols-2 gap-y-4 space-x-2 sm:grid-cols-2 sm:gap-x-6 lg:grid-cols-4 xl:gap-x-8">
            <slot />
            <!-- <div>
                <div class="relative">
                    <div class="relative h-72 w-full overflow-hidden rounded-lg">
                        <img src="https://tailwindui.com/img/ecommerce-images/product-page-03-related-product-01.jpg"
                            alt="Front of zip tote bag with white canvas, black canvas straps and handle, and black zipper pulls."
                            class="h-full w-full object-cover object-center">
                    </div>
                    <div class="relative mt-4">
                        <h3 class="text-sm font-medium text-gray-900">Zip Tote Basket</h3>
                        <p class="mt-1 text-sm text-gray-500">White and black</p>
                    </div>
                    <div
                        class="absolute inset-x-0 top-0 flex h-72 items-end justify-end overflow-hidden rounded-lg p-4">
                        <div aria-hidden="true"
                            class="absolute inset-x-0 bottom-0 h-36 bg-gradient-to-t from-black opacity-50">
                        </div>
                        <p class="relative text-lg flex space-x-2 items-center font-semibold text-white">
                            <span> 4.1</span> <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"
                                fill="currentColor" class="w-6 h-6">
                                <path fill-rule="evenodd"
                                    d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
                                    clip-rule="evenodd" />
                            </svg>
                        </p>
                    </div>
                </div>
                <div class="mt-6">
                  
                </div>
            </div>
             -->
        </div>
    </div>
</template>



