<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost"/>
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/admin/AdminPostForm';

export default {
  layout:'admin',
  components: {
    AdminPostForm,
    AdminPostForm
}, 
data() {
  return {
    loadedPost : {
      author: 'Test',
        title: 'Test', 
        thumbnailLink: 'Test',
        content: 'Test',
    }
  }
}
}

</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>