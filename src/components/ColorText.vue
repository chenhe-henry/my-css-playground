<template>
  <BaseCard>
    <h1 class="showcase colorText">Hello, this is a gradient text!!!</h1>
    <h2 class="title">Color Text</h2>
  </BaseCard>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.showcase {
  grid-column: 1/2;
  grid-row: 1/-1;
}
.title {
  grid-column: 2/-1;
  grid-row: 1/2;
}
.colorText {
  font-size: 3rem;
  font-weight: bold;
  background: linear-gradient(to right, red, blue, yellow, green);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
  background-size: 500%;
}
</style>
