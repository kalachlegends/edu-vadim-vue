<template>
  <div class="post">
    <div class="post__title">{{ title }}</div>
    <div class="post__description">{{ discription }}</div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    discription: String,
  },
  setup() {
    return {};
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
}
</style>
