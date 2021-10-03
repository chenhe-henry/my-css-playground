<template>
  <div>
    <h1>Gallery</h1>
    <div class="about">
      <ColorText /><BoxShadow /><MovingText /><Skeleton />
    </div>
  </div>
</template>
<script>
export default {
  components: {
    ColorText: () => import("@/components/ColorText.vue"),
    BoxShadow: () => import("@/components/BoxShadow.vue"),
    MovingText: () => import("@/components/MovingText.vue"),
    Skeleton: () => import("@/components/Skeleton.vue"),
  },
};
</script>
<style lang="scss" scoped>
.about {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-row-gap: 1.5rem;
}
</style>
