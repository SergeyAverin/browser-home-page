<template>
  <div
    class="bookmark-grid"
    :style="{ gridTemplateColumns: `repeat(${columns}, 1fr)` }"
  >
    <SiteBookmark href="/" text="sdf" />
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

export default {
  name: "BookmarkGrid",
  components: {
    SiteBookmark,
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
}
</style>
