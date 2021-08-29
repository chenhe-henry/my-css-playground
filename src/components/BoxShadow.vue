<template>
  <BaseCard
    ><h1 slot="showcase" class="showcase"></h1>
    <h2 slot="title" class="title">Negative Box Shadow</h2>
    <div slot="description" class="description">
      <div>Key Points:</div>
      <li>Multi box-shadow</li>
    </div>
  </BaseCard>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.showcase {
  height: 80%;
  width: 100%;
  border: 1px solid black;
  box-shadow: 0 20px 0 -10px red, 0 40px 0 -20px pink, 0 60px 0 -30px green,
    0 80px 0 -40px blue;
}
</style>
