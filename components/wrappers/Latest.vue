<template>
    <div class="flex flex-col w-full">
        <div class="flex w-full items-center pr-20">
            <label class="w-1/3 md:w-1/4 xl:w-1/6 text-lg text-gray-700 font-sans font-medium tracking-wide">Latest News</label>
             <div class="h-1 w-full bg-blue-600 px-8"></div>
        </div>
        <div class="flex flex-col py-10">
            <slot name="latest"></slot>
        </div>
    </div>
</template>