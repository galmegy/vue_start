<template>

  <div>
    <img :src="원룸.image" class='room-img'>
    <h4 >{{원룸.title}}</h4>
    <p>{{원룸.price}}원</p>
  </div>
  
</template>

<script>
export default {
    name: 'card-item',
    props: {  // 전달받은 항목 등록
        원룸: Object,
    },
    methods : {
    }
}
</script>

<style>

</style>