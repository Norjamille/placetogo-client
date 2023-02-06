
<script setup>
let props = defineProps({
    name: String,
    isBookMarked: Boolean,
    location: String,
    tags: Object,
    slug: String,
})

let viewRoute = "/places/" + props.slug
</script>
<template>
    <div class="max-w-sm group rounded-xl hover:scale-105 duration-150 ease-in-out overflow-hidden border relative">
        <button class="p-2 absolute top-2 right-2 rounded-full bg-gray-100">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                stroke="currentColor" class="w-4 h-4 text-gray-700">
                <path stroke-linecap="round" stroke-linejoin="round"
                    d="M17.593 3.322c1.1.128 1.907 1.077 1.907 2.185V21L12 17.25 4.5 21V5.507c0-1.108.806-2.057 1.907-2.185a48.507 48.507 0 0111.186 0z" />
            </svg>
        </button>
        <img class="w-full h-40 sm:h-72" src="https://source.unsplash.com/random/?city,night"
            alt="Sunset in the mountains">
        <div class="mt-2 px-2 flex space-x-1 items-center  overflow-hidden">
            <span
                class="inline-flex items-center rounded-full bg-gray-100 px-2.5 py-0.5 text-xs font-medium text-gray-600">
                Beach
            </span>
            <span
                class="inline-flex items-center rounded-full bg-gray-100 px-2.5 py-0.5 text-xs font-medium text-gray-600">
                Beach
            </span>
            <span
                class="inline-flex items-center rounded-full bg-gray-100 px-2.5 py-0.5 text-xs font-medium text-gray-600">
                Beach
            </span>
            <span
                class="inline-flex items-center rounded-full bg-gray-100 px-2.5 py-0.5 text-xs font-medium text-gray-600">
                Beach
            </span>
            <span
                class="inline-flex items-center rounded-full bg-gray-100 px-2.5 py-0.5 text-xs font-medium text-gray-600">
                Beach
            </span>
            <span
                class="inline-flex items-center rounded-full bg-gray-100 px-2.5 py-0.5 text-xs font-medium text-gray-600">
                Beach
            </span>
        </div>
        <div class="px-3.5 pt-3 pb-3.5">
            <div class="flex justify-between">
                <NuxtLink :to="viewRoute" class="text-sm group-hover:underline font-semibold">
                    Samal Island
                </NuxtLink>
            </div>
            <div class="flex mt-1 justify-between">
                <div class="flex text-gray-400">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-4 h-4">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z" />
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1115 0z" />
                    </svg>
                    <span class="text-xs ml-2">
                        Davao City
                    </span>
                </div>
                <div class="flex text-gray-400">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-4 h-4">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M11.48 3.499a.562.562 0 011.04 0l2.125 5.111a.563.563 0 00.475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 00-.182.557l1.285 5.385a.562.562 0 01-.84.61l-4.725-2.885a.563.563 0 00-.586 0L6.982 20.54a.562.562 0 01-.84-.61l1.285-5.386a.562.562 0 00-.182-.557l-4.204-3.602a.563.563 0 01.321-.988l5.518-.442a.563.563 0 00.475-.345L11.48 3.5z" />
                    </svg>
                    <span class="text-xs ml-2">
                        4.3
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

