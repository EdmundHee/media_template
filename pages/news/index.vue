<template>
    <div class="relative h-screen w-screen">
        <Navigation />
        <div class="h-screen w-screen outflow-y-auto pt-32 px-10">
            <div class="flex flex-col pr-20 items-center">
                <div class="h-full w-1/2 py-2">
                    <img :srcset="imgURL" class="h-full w-full object-cover"/>
                </div>
                <label>by {{authorName}}</label>
                <span class="text-2xl font-medium tracking-wide py-8">{{title}}</span>
                <div class="py-10 px-8">
                    <p class="text-lg font-sans tracking-wide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum distinctio voluptatem doloremque possimus commodi similique esse repellendus? Necessitatibus totam, molestiae quod quibusdam quos delectus tenetur ipsum nostrum modi sit cupiditate?</p>
                    <p class="text-lg font-sans tracking-wide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum distinctio voluptatem doloremque possimus commodi similique esse repellendus? Necessitatibus totam, molestiae quod quibusdam quos delectus tenetur ipsum nostrum modi sit cupiditate?</p>
                    <p class="text-lg font-sans tracking-wide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum distinctio voluptatem doloremque possimus commodi similique esse repellendus? Necessitatibus totam, molestiae quod quibusdam quos delectus tenetur ipsum nostrum modi sit cupiditate?</p>
                    <p class="text-lg font-sans tracking-wide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum distinctio voluptatem doloremque possimus commodi similique esse repellendus? Necessitatibus totam, molestiae quod quibusdam quos delectus tenetur ipsum nostrum modi sit cupiditate?</p>
                    <p class="text-lg font-sans tracking-wide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum distinctio voluptatem doloremque possimus commodi similique esse repellendus? Necessitatibus totam, molestiae quod quibusdam quos delectus tenetur ipsum nostrum modi sit cupiditate?</p>
                    <p class="text-lg font-sans tracking-wide">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum distinctio voluptatem doloremque possimus commodi similique esse repellendus? Necessitatibus totam, molestiae quod quibusdam quos delectus tenetur ipsum nostrum modi sit cupiditate?</p>
                </div>
                
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data: function(){
        return {
            title: this.$route.query.title,
            newsId: this.$route.query.id,
            imgURL: '/img/news.jpg',
            authorName: "Edmund"
        }
    }
}
</script>
