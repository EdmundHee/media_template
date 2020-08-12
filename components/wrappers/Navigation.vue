<template>
    <div class="absolute top-0 w-screen h-16">
        <div class="flex items-center justify-between py-3 px-10 bg-blue-600 shadow-navi">
            <div class="flex items-center">
                <img :srcset="logoURL" class="h-10 object-cover mx-8" />
                <div class="flex mx-10">
                    <nuxt-link to="" class="uppercase tracking-wide transition-all duration-500 ease-in-out text-gray-200 hover:text-white font-sans font-medium text-lg">news</nuxt-link>
                </div>
            </div>
            <div class="flex mx-8">
                <a href="#" target="_blank" class="mx-2 transition-all duration-500 ease-in-out text-gray-200 hover:text-white text-2xl"><i class="fab fa-facebook-f"></i></a>
                <a href="#" target="_blank" class="mx-2 transition-all duration-500 ease-in-out text-gray-200 hover:text-white text-2xl"><i class="fab fa-linkedin-in"></i></a>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        logoURL: {
            type: String,
            default: '/img/lead-white-logo.png'
        }
    }
}
</script>