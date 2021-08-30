<template>
  <BaseCard>
    <h1 slot="showcase" class="showcase">
      <div class="showcase-image"></div>
      <div class="showcase-title"></div>
      <div class="showcase-para">
        <div class="showcase-text"></div>
        <div class="showcase-text"></div>
        <div class="showcase-text"></div>
      </div>
    </h1>
    <h2 slot="title" class="title">Skeleton</h2>
    <div slot="description" class="description">
      <div>Key Points:</div>
      <li>keyframes</li>
    </div>
  </BaseCard>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.showcase {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 2fr;
  column-gap: 1rem;
  &-image,
  &-title,
  &-text {
    margin: 5px 0;
    animation: skeleton 3s infinite;
  }
  &-image {
    height: 100px;
    width: 100px;
    border-radius: 50%;
    grid-column: 1/2;
    grid-row: 1/2;
    justify-content: center;
    align-items: center;
    margin: auto 0;
  }

  &-title {
    height: 50px;
    width: 100%;
    grid-column: 2/-1;
    grid-row: 1/2;
    margin: auto 0;
  }
  &-para {
    grid-column: 1/-1;
    grid-row: 2/3;
    margin-top: 50px;
  }
  &-text {
    height: 20px;
    width: 100%;

    &:last-child {
      width: 70%;
    }
  }
  @keyframes skeleton {
    0% {
      background-color: hsl(0, 0%, 50%);
    }
    50% {
      background-color: hsl(0, 0%, 80%);
    }
    100% {
      background-color: hsl(0, 0%, 50%);
    }
  }
}
</style>
