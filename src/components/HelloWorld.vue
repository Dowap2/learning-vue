<template>
  <div class="hello">
    <h1>{{ msg }} {{ num }}</h1>
    {{ seen }}
    <p v-if="seen">원본 메시지</p>
    <li v-for="(item, i) in list" v-bind:key="item">{{ item }} {{ i }}</li>
    {{ obj }}
    <Post v-bind:post="{ id: 1, message: 'meesage' }" />
  </div>
</template>

<script>
import Post from "./Post.vue";
export default {
  name: "HelloWorld",
  components: {
    Post
  },
  props: {
    msg: String,
    num: Number,
    seen: Boolean,
    list: Array,
    obj: Object
  }
};
</script>
