<template>
  <div class="post">
    {{ post.id }}
    {{ post.message }}
  </div>
</template>

<script>
export default {
  name: "Post",
  props: {
    post: Object
  }
};
</script>
