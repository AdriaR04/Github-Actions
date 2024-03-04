<template>
  <div id="app">
    <div v-for="number in numbers" :key="number" class="key" @click="showNumber(number)">
      {{ number }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      numbers: [1, 2, 3, 4, 5, 6, 7, 8, 9],
    };
  },
  methods: {
    showNumber(number) {
      alert(`Has clicat el número: ${number}`);
    },
  },
};
</script>

<style>
.key {
  display: inline-block;
  padding: 10px;
  margin: 5px;
  background: #eee;
  cursor: pointer;
}
</style>

