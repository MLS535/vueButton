<template>
  <div>{{ counter }}</div>
  <button @click="incrementNumber">Increase</button>
  <button @click="reloadCounter">reload the counter</button>
</template>
<script>
export default {
  name: "ButtonIncrease",

  data() {
    return {
      counter: 0,
    };
  },
  methods: {
    incrementNumber: function () {
      this.counter++;
    },
    reloadCounter: function () {
      this.counter = 0;
    },
  },
};
</script>
<style scoped>
</style>