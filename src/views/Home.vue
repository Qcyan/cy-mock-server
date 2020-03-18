<template>
  <div class="home">
  2333

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import axios from 'axios'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  mounted() {
//    axios.get('/dev-api/transaction/list').then(()=> {
//
//    })


    axios.get('api/comment/get.action', {}).then((res) => {
      console.log(res.data)
    })

  }
}
</script>
