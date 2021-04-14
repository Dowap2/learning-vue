<template>
  <div class="hello">
    <h1>{{ msg }} {{ num }}</h1>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
    num: Number
  }
};
</script>
