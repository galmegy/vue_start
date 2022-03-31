<template>

  <Modal :원룸들="원룸들" :누른거="누른거" :모달창열렸니="모달창열렸니" />
  <Card :원룸="원룸들[i]" v-for="(a,i) in 원룸들" :key="i" />

</template>

<script>
import data from './assets/oneroom.js';
import Modal from './Modal.vue';
import Card from './Card.vue';

export default {
  name: 'App',
  data() {
    return {
      누른거: 0,
      원룸들: data,
      모달창열렸니 : true,
    }
  },  
  components: {  
    Modal: Modal,
    Card: Card,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
