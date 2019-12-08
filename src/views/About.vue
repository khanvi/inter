<template>
  <div class="about">
    <h1>This is an about page</h1>
    <p> masha</p>
    <Alesha/>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
import Alesha from '@/components/Menu.vue'

export default {
  name: 'home',
  components: {
    Alesha
  }
}
</script>

<style scoped>

p {
  color: #f00;
}
</style>
