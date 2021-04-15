<template>
  <div id="app">
    <HelloWorld msg="h" num="1" v-bind:seen="true" />
    <HelloWorld msg="he" num="2" v-bind:seen="false" />
    <HelloWorld msg="hel" num="3" v-bind:seen="false" />
    <HelloWorld msg="hell" num="4" v-bind:seen="false" />
    <HelloWorld msg="hello" num="5" v-bind:seen="true" />
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
