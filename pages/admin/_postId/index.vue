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