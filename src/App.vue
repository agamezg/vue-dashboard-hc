<template>
  <div id="app">
    <WaterTank percentage=56 identifier="Rudy's"></WaterTank>
    <WaterTank percentage=82 identifier="Raquel's"></WaterTank>
  </div>
</template>

<script>
import WaterTank from "@/components/WaterTank";

export default {
  name: 'App',
  components: {
    WaterTank
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: #2c3e50;
  margin-top: 60px;
  display: flex;
  justify-content: center;
}

h1 {
  font-size: large;
  color: white;
}

h2 {
  font-size: medium;
  color: #2c3e50;
}
</style>
