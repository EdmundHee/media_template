<template>
    <div class="flex flex-col w-full">
        <div class="flex w-full items-center">
            <label class="w-full text-lg text-gray-700 font-sans font-medium tracking-wide">Social Media</label>
             <div class="h-1 w-full bg-blue-600 px-8"></div>
        </div>
        <div class="flex py-10 grid grid-cols-4 gap-1">
            <slot name="social"></slot>
        </div>
    </div>
</template>
<script>
export default {
    props:{
        fbURL:{
            type: String,
            default: 'https://facebook.com'
        },
        inURL:{
            type: String,
            default: 'https://linkedin.com'
        }
    }
}
</script>