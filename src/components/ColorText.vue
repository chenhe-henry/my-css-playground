<template>
  <BaseCard>
    <h1 slot="showcase" class="showcase">Hello, this is a gradient text!!!</h1>
    <h2 slot="title" class="title">Gradient Color Text</h2>
    <div slot="description" class="description">
      <div>Key Points:</div>
      <li>background: linear-gradient</li>
      <li>background-clip: text</li>
    </div>
  </BaseCard>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.showcase {
  font-size: 3rem;
  font-weight: bold;
  background: linear-gradient(to right, red, blue, yellow, green);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
  background-size: 500%;
}
</style>
