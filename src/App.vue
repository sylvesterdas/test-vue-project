<template>
  <div>
    <MyButton @click="onClick" />
    <MyCounter :counter="counter" />
  </div>
</template>

<script>
import MyCounter from "@/components/MyCounter";
import MyButton from "@/components/MyButton";

export default {
  name: "App",
  components: {
    MyCounter,
    MyButton,
  },
  data: function () {
    return {
      counter: 0,
    };
  },
  methods: {
    onClick: function () {
      this.counter++;
    },
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding-top: 40px;
  padding-left: 4px;
  padding-right: 4px;
  background-color: gray;
  height: 100vh;
}
</style>
