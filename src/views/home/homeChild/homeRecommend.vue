<template>
  <div class="recommend">
    <div v-for="items in recommend" class="recommend-item">
      <a :href="items.link">
      <img :src="items.image" alt="">
      <div> {{items.title}} </div>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'homeRecommend',
  props: {
    recommend: {
      type: Array,
      default(){
        return []
      }
    }
  }
}
</script>

<style >
.recommend{
display: flex;
text-align: center;
padding: 10px 0 30px;
border-bottom: 8px solid #eee;
}
.recommend-item{
  flex: 1;
}
.recommend-item img{
  wideh: 65px;
  height: 65px;
  margin-bottom: 4px;
}
</style>
