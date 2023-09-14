<template>
  <section class="featured-posts">
      <PostPreview id="1" thumbnail="https://www.afterschoolafrica.com/wp-content/uploads/2020/03/Technology-industry-720x430-1.jpg" title="Hello There" previewText="My first post"/>
      <PostPreview id="2" thumbnail="https://www.afterschoolafrica.com/wp-content/uploads/2020/03/Technology-industry-720x430-1.jpg" title="Hello There" previewText="My first post"/>
      <PostPreview id="3" thumbnail="https://www.afterschoolafrica.com/wp-content/uploads/2020/03/Technology-industry-720x430-1.jpg" title="Hello There" previewText="My first post"/>
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: { PostPreview }
}
</script>

<style scoped>
 .featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>