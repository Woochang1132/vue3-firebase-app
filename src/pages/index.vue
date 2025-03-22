<template>
  <q-page padding>
    <div class="text-h4">커뮤니티 목록</div>
    <section class="q-gutter-y-sm q-mt-lg">
      <PostList :items="posts"></PostList>
    </section>
  </q-page>
</template>

<script setup>
import PostList from 'src/components/apps/post/PostList.vue';
// import { useRouter } from 'vue-router';

// const router = useRouter();
// const goPostDetails = id => {
//   router.push(`/posts/${id}`);
// };

const posts = Array.from(Array(20), (_, index) => ({
  id: index,
  title: 'Vue3 Firebase 강의' + index,
}));
</script>

<style lang="scss" scoped></style>
