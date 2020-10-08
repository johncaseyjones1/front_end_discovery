<template>
  <div>
    <div id="cpu">
      <h1>User Page</h1>
      <Build/>
    </div>
  </div>
</template>

<script>
import Build from "../components/build.vue"

export default {
  name: 'user',
  components: {
    Build
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
