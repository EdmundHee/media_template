<template>
    <div class="flex flex-col py-4 px-2">
        <img :srcset="newsURL" />
        <div class="flex flex-col w-full py-4 px-6">
            <nuxt-link :to="pageURL" class="transition-all duration-500 ease-in-out text-gray-800 hover:text-black text-xl text-center tracking-wide font-sans">{{newsTitle}}</nuxt-link>
            <div class="text-center mt-2 transition-all duration-500 ease-in-out text-gray-800 hover:text-black cursor-pointer">
                by {{authorName}}
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props : {
        newsURL: {
            type: String,
            default: '/img/news.jpg'
        },
        pageURL: {
            type: String,
            default: '/news'
        },
        newsTitle: {
            type: String,
            default: 'News Title'
        },
        authorName: {
            type: String,
            default: "Author Name"
        }
    }
}
</script>