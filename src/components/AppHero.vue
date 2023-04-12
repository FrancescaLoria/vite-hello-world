<script>
export default {
  data() {
    return {
      myImg: "img.jpg",
    };
  },
  methods: {
    getImgUrl() {
      return new URL(`../assets/${this.myImg}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div>
    <img :src="getImgUrl()" alt="adventure-time" />
  </div>
</template>

<style></style>
