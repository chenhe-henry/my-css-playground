<template>
  <div class="card">
    <slot></slot>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.card {
  height: 25vh;
  width: 40vw;
  background: white;
  margin: 0 5vw;
  display: grid;
  grid-template-columns: 2fr 1fr;
  grid-template-rows: 1fr 1fr;
  border-radius: 10px;
  box-shadow: 10px 10px 5px 0 black;
}
</style>
