<template>
  <div class="h-full w-full">
    <Navigation/>
    <div class="h-screen w-screen pt-20">
      <!-- FEATURED NEWS -->
      <Feature class="px-10">
        <template v-slot:featured>
          <FeatureNews
            newsURL="https://images.pexels.com/photos/285814/pexels-photo-285814.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
            newsTitle="News Title One"
            pageURL="/news?title=News Title One&id=12345"
            authorName="Author 1 @ LEAD"
          />
          <FeatureNews
            newsURL="https://images.pexels.com/photos/35550/ipad-tablet-technology-touch.jpg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
            newsTitle="Featured News"
            pageURL="/news?title=Featured News&id=12346"
            authorName="Edmund Hee"
          />
          <FeatureNews
            newsURL="/img/news.jpg"
            newsTitle="News Title three"
            pageURL="/news?title=News Title three&id=12347"
            authorName="Edmund Hee"
          />
        </template>
      </Feature>

      <!-- LATEST NEWS & SOCIAL MEDIA -->
      <div class="flex flex-col md:flex-row px-10">
        <div class="w-full md:w-1/2 lg:w-2/3">
          <Latest>
            <template v-slot:latest>
              <LatestNew
                newsURL="/img/news.jpg"
                newsTitle="News Title 4"
                pageURL="/news?title=News Title 4&id=12347"
                authorName="Edmund Hee"
              />
              <LatestNew
                newsURL="/img/news.jpg"
                newsTitle="News Title 5"
                pageURL="/news?title=News Title 5&id=12349"
                authorName="Edmund Hee"
              />
            </template>
          </Latest>
        </div>
        <div class="w-full md:w-1/2 lg:w-1/3">
          <!-- SOCIAL MEDIA SIDE -->
          <Social>
            <template v-slot:social>
              <SocialButton class="bg-blue-600 hover:bg-blue-700" URL="https://facebook.com">
                <template v-slot:icon>
                  <i class="fab fa-facebook-f"></i>
                </template>
              </SocialButton>
              <SocialButton class="bg-blue-400 hover:bg-blue-500" URL="https://linkedin.com">
                <template v-slot:icon>
                  <i class="fab fa-linkedin-in"></i>
                </template>
              </SocialButton>
            </template>
          </Social>
        </div>
      </div>
      <Footer/>
    </div>
  </div>
</template>

<script>
export default {};
</script>
