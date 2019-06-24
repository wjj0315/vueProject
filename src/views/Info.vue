<template>
  <div>
    hello Info Component
    <button type="button" @click="add()">添加</button>
  </div>
</template>
<script>
import store from "@/store";
export default {
  name: "Info",
  store,
  data() {
    return {
      // msg:store.state.count
    };
  },
  mounted() {
  },
  methods: {
    add() {
      console.log("add event from info!");
      // debugger
      store.commit("increase");
    },
   
  }
};
</script>
<style scoped>
</style>


