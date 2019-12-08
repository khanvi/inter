<template>
  <div class="home">
    {{ counter }}
    <Alesha @click.native="quak(2)"/>
    <div v-show="counter > 4">
      SHhowing test
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
import Alesha from '@/components/Menu.vue'

export default {
  name: 'home',
  components: {
    //HelloWorld,
    Alesha
  },
  data: function() {
    return {
      hello: 'Привет пользователь',
      counter: 0
    }
  },
  methods: {
    quak: function(num) {
      this.counter += num 
      // eslint-disable-next-line
      console.log(99)
    }
  },
  created: function() {
      // eslint-disable-next-line
      console.log('creTATE')
    },
  mounted: function() {
      // eslint-disable-next-line
      console.log('start')
    }
 }
</script>
