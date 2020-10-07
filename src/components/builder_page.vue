<template>
  <div>
    <div id="cpu">
      <h1>Builder Page</h1>
      <CPUSs/>
      <MOBOs/>
      <Coolers/>
    </div>
  </div>
</template>

<script>
import CPUSs from "../components/cpus.vue"
import MOBOs from "../components/motherboards.vue"
import Coolers from "../components/coolers.vue"

export default {
  name: 'HelloWorld',
  components: {
    CPUSs,
    MOBOs,
    Coolers
  },
  props: {
  }
}
</script>

<style>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.component_label {
  background-color: #4c63af; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
</style>
