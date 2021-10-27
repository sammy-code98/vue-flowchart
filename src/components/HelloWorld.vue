<template>
  <div class="container-xl my-contain">
    <carousel />
    <flowchart />
    <br />
    <br />
    <flow class="my-margin" />
  </div>
</template>

<script>
import flowchart from "./FlowChart.vue";
import flow from "./Flow.vue";
import carousel from "./Carousel.vue";
export default {
  name: "HelloWorld",
  components: {
    flowchart,
    flow,
    carousel,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.my-contain {
  margin-top: 10px;
}
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
.my-margin {
  margin: auto;
  padding: 30px;
}
</style>
