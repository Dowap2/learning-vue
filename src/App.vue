<template>
  <div id="app">
    <HelloWorld msg="h" num="1" />
    <HelloWorld msg="he" num="2" />
    <HelloWorld msg="hel" num="3" />
    <HelloWorld msg="hell" num="4" />
    <HelloWorld msg="hello" num="5" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld
  }
};
</script>
