<template>
  <h1>APP</h1>
  <SiteBookmark href="https://www.deepl.com/translator#en/ru/Site%20Bookmark" text="tt" />
</template>

<script>
import SiteBookmark from './components/SiteBookmark.vue';

export default {
  name: 'App',
  components: {
    SiteBookmark,
  }
}
</script>

<style>
  body {
    background: #101211;
    color: #fff;
  }
</style>
