<template>
  <div class="relative h-screen w-screen">
    <Navigation />
    <div class="h-screen w-screen outflow-y-auto pt-20 px-10">
      <!-- FEATURED NEWS -->
      <Feature>
        <template v-slot:featured>
          <FeatureNews 
            newsURL="/img/news.jpg"
            newsTitle="News Title One"
            pageURL="/news?title=News Title One&id=12345"
            authorName="Edmund Hee"/>
          <FeatureNews 
            newsURL="/img/news.jpg"
            newsTitle="News Title Two"
            pageURL="/news?title=News Title Two&id=12346"
            authorName="Edmund Hee"/>
          <FeatureNews 
            newsURL="/img/news.jpg"
            newsTitle="News Title three"
            pageURL="/news?title=News Title three&id=12347"
            authorName="Edmund Hee"/>
        </template>
      </Feature>

      <!-- LATEST NEWS & SOCIAL MEDIA -->
      <div class="flex flex-col md:flex-row">
        <div class="w-full md:w-1/2 lg:w-2/3">
          <Latest>
            <template v-slot:latest>
              <LatestNew 
                newsURL="/img/news.jpg"
                newsTitle="News Title 4"
                pageURL="/news?title=News Title 4&id=12347"
                authorName="Edmund Hee"/>
              <LatestNew 
                newsURL="/img/news.jpg"
                newsTitle="News Title 5"
                pageURL="/news?title=News Title 5&id=12349"
                authorName="Edmund Hee"/>
            </template>
          </Latest>
        </div>
        <div class="w-full md:w-1/2 lg:w-1/3">
        <!-- SOCIAL MEDIA SIDE -->
          <Social>
            <template v-slot:social>
              <SocialButton class="bg-blue-600 hover:bg-blue-700" :URL='fbURL'><template v-slot:icon><i class="fab fa-facebook-f"></i></template></SocialButton>
              <SocialButton class="bg-blue-400 hover:bg-blue-500" :URL='inURL'><template v-slot:icon><i class="fab fa-linkedin-in"></i></template></SocialButton>
            </template>
          </Social>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
export default {}
</script>
