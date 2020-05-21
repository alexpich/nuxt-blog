<template>
  <div class="posts-page">
    <PostList :posts="loadedPosts" />
  </div>
</template>

<script>
import PostList from "@/components/Posts/PostList";
export default {
  components: {
    PostList
  },
  asyncData(context, callback) {
    setTimeout(() => {
      callback(null, {
        loadedPosts: [
          {
            id: "1",
            title: "first post",
            previewText: "This my first posty post.",
            thumbnail:
              "https://icatcare.org/app/uploads/2018/07/Thinking-of-getting-a-cat.png"
          },
          {
            id: "2",
            title: "second post",
            previewText: "This my second posty post.",
            thumbnail:
              "https://icatcare.org/app/uploads/2018/07/Thinking-of-getting-a-cat.png"
          }
        ]
      });
    }, 1500);
  }
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
