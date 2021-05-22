<template>
  <div>
    a
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
