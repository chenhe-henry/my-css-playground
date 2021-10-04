<template>
  <button class="baseBtn" @click="clickBtn">
    {{ text }}
  </button>
</template>

<script>
export default {
  props: { text: { type: String, required: true } },
  methods: {
    clickBtn() {
      this.$emit("clicked");
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/custom.scss";
.baseBtn {
  cursor: pointer;
  position: relative;
  font-family: monospace;
  border-radius: 15em;
  border: none;
  box-shadow: 0 0 2px 2px $white;
  background-color: $white;
  padding: 1rem;
  transition: all 0.75s;

  &:hover {
    transition: all 0.75s;
    background: darken($color: $white, $amount: 10%);
    box-shadow: 0 0 2px 2px darken($color: $white, $amount: 10%);
    transform: translateY(-0.25rem);
  }
  &:active {
    transform: translateY(0);
  }
}
</style>
