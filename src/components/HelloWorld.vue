<template>
  <div class="hello">
    <h1>{{ msg }} {{ num }}</h1>
    <p v-if="seen">원본 메시지{{ seen }}</p>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
    num: Number,
    seen: Boolean
  }
};
</script>
