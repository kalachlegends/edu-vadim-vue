<template>
  <div class="post">
    <div class="post__title">{{ title }}</div>
    <div class="post__description">{{ discription }}</div>
    <div v-if="img" class="post__img">
      <img :src="img">
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    discription: String,
    img: String
},
};
</script>

<style lang="scss" scoped>
.post {
  padding: 10px;
  background: white;
  color: black;
  &__title {
    font-weight: bold;
    font-size: 20px;
  }
  &__description {
    font-weight: normal;
    font-size: 15px;
  }
  &__img {
    width: 100px;
    height: 100px;
  }
}
</style>
