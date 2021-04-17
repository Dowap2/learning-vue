<template>
  <div id="app">
    <HelloWorld msg="h" num="1" v-bind:seen="true" v-bind:list="[1, 2]" />
    <HelloWorld
      msg="he"
      num="2"
      v-bind:seen="false"
      v-bind:list="['사과', '바나나']"
    />
    <HelloWorld
      msg="hel"
      num="3"
      v-bind:seen="false"
      v-bind:obj="{ message: 'object', anotherMessage: 'hello' }"
    />
    <HelloWorld msg="hell" num="4" v-bind:seen="false" />
    <HelloWorld msg="hello" num="5" v-bind:seen="true" />
    {{ message }}
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
