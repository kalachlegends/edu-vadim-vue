<script>
import postVue from "./components/post.vue";

export default {
  data: () => ({ count: 0, imgUrl: "/src/assets/vue.svg"}),
  components: { postVue },
  methods: {
    handleCLick: function (e) {
      console.log(this);
    },
    handleCLickTwo: function (e) {
      console.log(this.count);
      this.count++;
    },
  }
}
</script>

<template>
  <postVue v-if="count > 2" :title="count" discription="'2'" />
  <div>Я появился</div>
  <div @click="handleCLick">Я event handleCLick</div>
  <div @click="handleCLickTwo">Я event handleCLickTwo</div>
  <postVue :img="imgUrl" />
</template>

<style scoped></style>
