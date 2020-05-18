<template>
  <section class="post-list">
    <PostPreview
      id="1"
      thumbnail="https://icatcare.org/app/uploads/2018/07/Thinking-of-getting-a-cat.png"
      title="Hello there"
      previewText="First post"
    />
    <PostPreview
      id="2"
      thumbnail="https://icatcare.org/app/uploads/2018/07/Thinking-of-getting-a-cat.png"
      title="Hello there"
      previewText="Second post"
    />
    <PostPreview
      id="3"
      thumbnail="https://icatcare.org/app/uploads/2018/07/Thinking-of-getting-a-cat.png"
      title="Hello there"
      previewText="Third post"
    />
  </section>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";
export default {
  components: {
    PostPreview
  }
};
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>