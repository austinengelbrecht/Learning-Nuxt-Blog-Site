
<template>
  <div class="posts-page">
    <PostList :posts="loadedPosts" />
  </div>
</template>

<script>
import PostList from '@/components/Posts/PostList.vue';

export default {
  components: {
    PostList
  }, 
  asyncData(context){
    return new Promise((resolve, reject) =>{
      setTimeout(()=> {

        resolve({ loadedPosts: 
          [
            { id: '1', title: 'First Post', previewText: 'First Post', thumbnail: 'https://picsum.photos/200/300' },
            { id: '2', title: 'Second Post', previewText: 'Second Post', thumbnail: 'https://picsum.photos/200/300' },
          ]
        })
      },1000) ;
    }).then(data => {
      return data
    })
    .catch((e)=>{
      context.error(new Error())
    })
    
  }
}
</script>

<style scoped>
.post-page {
  display: flex;
  justify-content: center;
  align-items: center;
}


</style>