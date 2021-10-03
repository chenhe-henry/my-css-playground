<template>
  <button class="btn" @click="clickBtn">
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

<style lang="scss" scoped></style>
