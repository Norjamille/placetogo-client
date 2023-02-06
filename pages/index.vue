<script setup>

</script>
<template>
    <NuxtLayout name="user-layout">
        <div class="flex flex-col space-y-5">
            <div class="flex sm:justify-end ">
                <div class="relative">
                    <input type="search" placeholder="search"
                        class="rounded-full w-full border-0 bg-gray-100   focus:ring-0 pl-10 shadow-sm" />
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="absolute left-3 top-2 text-gray-400 w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
                    </svg>
                </div>
            </div>
            <SectionPanel title="Top Rated">
                <template #icon>
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-6 h-6 text-indigo-700">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M9 12h3.75M9 15h3.75M9 18h3.75m3 .75H18a2.25 2.25 0 002.25-2.25V6.108c0-1.135-.845-2.098-1.976-2.192a48.424 48.424 0 00-1.123-.08m-5.801 0c-.065.21-.1.433-.1.664 0 .414.336.75.75.75h4.5a.75.75 0 00.75-.75 2.25 2.25 0 00-.1-.664m-5.8 0A2.251 2.251 0 0113.5 2.25H15c1.012 0 1.867.668 2.15 1.586m-5.8 0c-.376.023-.75.05-1.124.08C9.095 4.01 8.25 4.973 8.25 6.108V8.25m0 0H4.875c-.621 0-1.125.504-1.125 1.125v11.25c0 .621.504 1.125 1.125 1.125h9.75c.621 0 1.125-.504 1.125-1.125V9.375c0-.621-.504-1.125-1.125-1.125H8.25zM6.75 12h.008v.008H6.75V12zm0 3h.008v.008H6.75V15zm0 3h.008v.008H6.75V18z" />
                    </svg>
                </template>
                <template #action>
                    <a href="#"
                        class="group inline-flex items-center rounded-full text-gray-500  px-3 py-1  text-xs font-semibold  transition">
                        <span class="hidden sm:block"> See More</span>
                        <svg class="mt-0.5 ml-2 -mr-1   stroke-gray-500 stroke-2" fill="none" width="10" height="10"
                            viewBox="0 0 10 10" aria-hidden="true">
                            <path class="opacity-0 transition group-hover:opacity-100" d="M0 5h7"></path>
                            <path class="transition group-hover:translate-x-[3px]" d="M1 1l4 4-4 4"></path>
                        </svg>
                    </a>
                </template>
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
            </SectionPanel>

            <SectionPanel title="Restaurants">
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
            </SectionPanel>
            <SectionPanel title="Coffee Shops">
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
                <PlaceCard slug="test-place" />
            </SectionPanel>
        </div>
    </NuxtLayout>
</template>