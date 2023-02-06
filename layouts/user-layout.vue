<script setup>

</script>

<template>
    <div class="relative isolate h-full bg-white">
        <div class="px-6  py-3 sm:py-6 lg:px-8 z-50 bg-white/70 backdrop-blur-sm sticky top-0">
            <Navigations />
        </div>
        <div class="mx-auto max-w-7xl px-6 py-10 sm:py-5  lg:flex lg:items-center lg:gap-x-10 lg:px-8 ">
            <slot />
        </div>
    </div>
</template>