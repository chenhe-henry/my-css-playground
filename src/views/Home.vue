<template>
  <div class="home">
    <ColorText />
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: { ColorText: () => import("@/components/ColorText.vue") },
};
</script>
<style lang="scss" scoped>
.home {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
</style>
