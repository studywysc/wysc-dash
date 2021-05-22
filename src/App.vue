<template>
  <div class="bg-gray-600 min-h-screen overflow-hidden">
    <div class="h-appbody grid grid-cols-3 bg-cover bg-center bg-fixed animate-fade-in-up" :style="{ backgroundImage: 'url(' + unsplashUrl + unsplashKeyword + ')' }">
      <!-- Left -->
      <div class="h-appbody">
        AA
      </div>

      <!-- Center -->
      <main>
        <router-view/>
      </main>

      <!-- Right -->
      <div>
        C
      </div>
    </div>
    <div class="h-appbarbottom">
      Hi
    </div>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        unsplashUrl: "https://source.unsplash.com/featured/1600x900/daily/?",
        unsplashKeyword: "nature"
      }
    },
    methods: {
      enterApp() {
        window.scrollTo({top: 0, behavior: 'smooth'});
      },
    },
  }
</script>
