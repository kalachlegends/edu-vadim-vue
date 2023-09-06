<script>
import postVue from "./components/post.vue";

export default {
  data: () => ({ count: 0 }),
  components: { postVue },
  methods: {
    handleCLick: function (e) {
      console.log(this);
    },
    handleCLickTwo: function (e) {
      console.log(this.count++);
    },
  },
};
</script>

<template>
  <postVue v-if="count > 2" :title="count" discription="'2'" />
  <div>Я появился</div>
  <div @click="handleCLick">Я event handleCLick</div>
  <div @click="handleCLickTwo">Я event handleCLickTwo</div>
  <!-- HINTS for 1: <img src="/vite.svg" /> -->
</template>

<style scoped></style>
