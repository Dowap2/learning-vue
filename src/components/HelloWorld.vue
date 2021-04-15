<template>
  <div class="hello">
    <h1>{{ msg }} {{ num }}</h1>
    {{ seen }}
    <p v-if="seen">원본 메시지</p>
    <li v-for="(item, i) in list">{{ item }} {{ i }}</li>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
    num: Number,
    seen: Boolean,
    list: Array
  }
};
</script>
