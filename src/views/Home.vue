<template>
  <div class="home"><ColorText /><BoxShadow /><MovingText /><Skeleton /></div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {
    ColorText: () => import("@/components/ColorText.vue"),
    BoxShadow: () => import("@/components/BoxShadow.vue"),
    MovingText: () => import("@/components/MovingText.vue"),
    Skeleton: () => import("@/components/Skeleton.vue"),
  },
};
</script>
<style lang="scss" scoped>
.home {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-row-gap: 1.5rem;
}
</style>
