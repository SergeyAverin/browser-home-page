<template>
  <div
    class="center-block"
    :style="{
      justifyContent: horizontal  && 'center',
      alignItems: vertikal && 'center',
    }"
  >
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: "CenterBlock",
  props: {
    horizontal: { type: Boolean },
    vertikal: { type: Boolean },
  },
};
</script>
<style>
.center-block {
  display: flex;
  position: fixed;
  width: 100%;
  height: 100%;
}
</style>
