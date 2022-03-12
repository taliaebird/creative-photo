<template>
  <div class="about page">
    <button v-on:click='select(13)'><img class='button-img' src='../assets/main-13.jpeg'/></button>
    <button v-on:click='select(12)'><img class='button-img' src='../assets/main-12.jpeg'/></button>
    <button v-on:click='select(6)'><img class='button-img' src='../assets/main-6.jpeg'/></button>
    <button v-on:click='select(8)'><img class='button-img' src='../assets/main-8.jpeg'/></button>
    <button v-on:click='select(7)'><img class='button-img' src='../assets/main-7.jpeg'/></button>
    <button v-on:click='select(10)'><img class='button-img' src='../assets/main-10.jpeg'/></button>
    <button v-on:click='select(9)'><img class='button-img' src='../assets/main-9.jpeg'/></button>
    <button v-on:click='select(5)'><img class='button-img' src='../assets/main-5.jpeg'/></button>
    <button v-on:click='select(11)'><img class='button-img' src='../assets/main-11.jpeg'/></button>
  </div>
</template>

<script>
export default {
  name: 'PortfolioItems',
  methods: {
    select(img) {
      console.log(this.$parent.$root._data.votes);

      this.$parent.$root._data.votes[img-1] += 1;
      console.log(this.$parent.$root._data.votes);
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
button {
  height: 33.333%;
  width: 33.333%;
  border: 0px;
}
.button-img {
  height: 100%;
  width: 100%;
}
.button:hover {
  border: red 1px solid;
}
</style>
