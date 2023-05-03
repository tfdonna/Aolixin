<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <HelloWorld/>
    <!-- <MySwiper></MySwiper> -->
    
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
//import MySwiper from '@/components/MySwiper'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
  }
}
</script>
<style scoped>
body{
  margin: 0;
  padding: 0;
  top: 0;
}
</style>