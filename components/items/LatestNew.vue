<template>
    <div class="flex flex-col md:flex-row w-full py-2 px-4">
        <img :srcset="newsURL" class="h-48 object-cover"/>
        <div class="flex flex-col py-4 px-2">
            <nuxt-link :to="pageURL" class="transition-all duration-500 ease-in-out text-gray-800 hover:text-black text-xl text-center md:text-left tracking-wide font-sans">{{newsTitle}}</nuxt-link>
            <label class="text-gray-800 hover:text-black text-center md:text-left tracking-wide font-sans">The school students and staff have been given two days off to</label>
            <label class="text-center md:text-left mt-2 transition-all duration-500 ease-in-out text-gray-800 hover:text-black cursor-pointer">
                by {{authorName}}
            </label>
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