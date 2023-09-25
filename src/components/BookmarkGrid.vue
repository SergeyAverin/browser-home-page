<template>
  <div
    class="bookmark-grid"
    :style="{ gridTemplateColumns: `repeat(${columns}, 1fr)` }"
  >
    <SearchWidget></SearchWidget>
    <SearchWidget></SearchWidget>
    <SiteBookmark href="/123" text="sdf" />
    <SiteBookmark href="/" text="sdf" />
    <SiteBookmark href="/" text="sdf" />
    <SiteBookmark href="/" text="sdf" />
    <SiteBookmark href="/" text="sdf" />
    <SiteBookmark href="/" text="sdf" />
    <SiteBookmark href="/" text="sdf" />
    <SiteBookmark href="/" text="sdf" />
    <SiteBookmark href="/" text="sdf" />
  </div>
</template>
<script>
import SiteBookmark from "./SiteBookmark.vue";
import SearchWidget from "./SearchWidget.vue";

export default {
  name: "BookmarkGrid",
  components: {
    SiteBookmark,
    SearchWidget
  },
  props: {
    columns: {
      type: Number,
    },
    rows: {
      type: Number,
    },
  },
};
</script>
<style>
.bookmark-grid {
  display: grid;
  width: 780px;
  height: 780px;
  grid-gap: 15px;
}
</style>
