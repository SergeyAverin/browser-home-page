<template>
  <h1>APP</h1>
  <BookmarkGrid columns="3" />
</template>

<script>
import BookmarkGrid from './components/BookmarkGrid.vue';

export default {
  name: 'App',
  components: {
    BookmarkGrid,
  }
}
</script>

<style>
  body {
    background: #101211;
    color: #fff;
  }
</style>
