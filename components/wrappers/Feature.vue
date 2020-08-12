<template>
<div class="flex flex-col">
    <div class="flex w-full px-2 items-center">
        <div class="h-1 w-full bg-blue-600 px-8"></div>
        <label class="w-full md:w-1/2 xl:w-1/3 text-center text-xl text-gray-700 font-sans font-medium tracking-wide">Featured News</label>
        <div class="h-1 w-full bg-blue-600 px-8"></div>
    </div>
    <div class="w-full grid grid-cols-1 md:grid-cols-3 gap-2">
            <slot name="featured"></slot>
    </div>
</div>
</template>