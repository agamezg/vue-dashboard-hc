<template>
  <div id="container">
    <div id="tank">
      <div v-bind:style="{height: percentage + '%'}" id="water">
        <h1>{{ percentage }}%</h1>
      </div>
    </div>
    <h2>{{ identifier }}</h2>
  </div>
</template>

<script>
export default {
  name: "WaterTank",
  props: {
    percentage: String,
    identifier: String
  }
}
</script>

<style scoped>
#container {
  height: 200px;
  width: 50%;
  display: flex;
  flex-direction: column;
  margin: 2%;
  justify-content: center;
  align-items: center;
}
#tank {
  background-color: darkgray;
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  border-radius: 10%;
  margin: auto;
}

#water {
  background-color: #2c3e50;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
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