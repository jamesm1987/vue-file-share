<template>
  <div class="w-full md:w-8/2 lg:w-6/12 mx-auto px-6 mt-6 md:mt-20">
    <Navigation />    
    <router-view />
  </div>
</template>

<script>
  import '@/assets/styles/app.css'
  import Navigation from '@/components/Navigation.vue'
  export default {
    components: {
      Navigation
    }
  }
</script>

