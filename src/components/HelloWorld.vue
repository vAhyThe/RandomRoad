<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <forward />
    <left />
    <right />
  </div>
</template>

<script>
import Forward from "./forward";
import Left from "@/components/left";
import Right from "@/components/right";
export default {
  name: "HelloWorld",
  components: {
    Right,
    Left,
    Forward,
  },
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
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
</style>
