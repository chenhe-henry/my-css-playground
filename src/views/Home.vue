<template>
  <div class="home">
    <div class="title content">Hello, I'm Henry He.</div>
    <div class="text content">Welcome to my CSS playground ^_^</div>
    <BaseButton text="Discovery More" @clicked="NavToGallery" class="btn" />
  </div>
</template>

<script>
export default {
  methods: {
    NavToGallery() {
      this.$router.push({ name: "Gallery" });
    },
  },
};
</script>
<style lang="scss" scoped>
@import "../assets/scss/custom.scss";
.content {
  color: $white;
  font-weight: bold;
  text-align: left;
}
.title {
  font-size: 3rem;
  font-family: monospace;
  position: relative;
  width: max-content;
  &::before,
  &::after {
    content: "";
    position: absolute;
    inset: 0;
  }
  &::before {
    background: $bg-dark;
    animation: typewriter $typewriterSpeed steps(20) 1s forwards;
  }
  &::after {
    width: 0.125em;
    background: $white;
    animation: typewriter $typewriterSpeed steps(20) 1s forwards,
      blink 750ms steps(20) infinite;
  }
}
.text,
.btn {
  opacity: 0;
  transform: translateY(3rem);
  animation: fadeInUp 2s ease $typewriterSpeed + 2s forwards;
}
.text {
  font-size: 1.5rem;
}
.home {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
