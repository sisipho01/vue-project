<template>
  <div class="home">
  <p class="italic">Hallo, Sanibonani, Molweni, Thobela, Dumela, Lumela, Abusheni, Sanibona, Avuwani, Salibonani, Hello welcome to my Portfolio!</p>

  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
<style scoped>

.italic{
  font-family:cursive;
  font-size: large;
}
.home {
  background-image: url('https://i.postimg.cc/wvCnNFN3/a.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
  min-height: 100vh;
  color: white;
}

</style>