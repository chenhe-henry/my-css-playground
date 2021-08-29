<template>
  <div class="card">
    <slot name="showcase" class="showcase"></slot>
    <slot name="title" class="title"></slot>
    <slot name="description" class="description"></slot>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.card {
  background: white;
  margin: 0 5vw;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  border-radius: 10px;
  box-shadow: 10px 10px 5px 0 black;
  padding: 2em;
  text-align: left;
  & > * {
    margin: 0 auto;
  }
}
.showcase {
  grid-column: 1/2;
  grid-row: 1/-1;
}
.title {
  grid-column: 2/-1;
  grid-row: 1/2;
}
.description {
  grid-column: 2/-1;
  grid-row: 2/-1;
  text-align: left;
}
</style>
