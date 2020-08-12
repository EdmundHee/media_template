<template>
    <a :href="URL" target="_blank" class="transition-all duration-500 ease-in-out py-2 px-12 hover:text-white text-gray-200">
        <slot name="icon"></slot>
    </a>
</template>
<script>
export default {
    props: {
        URL: {
            type: String,
            default: 'https://google.com'
        }
    }
}
</script>