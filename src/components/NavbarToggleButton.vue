<template>
  <button
    class="navbar-toggler"
    type="button"
    data-toggle="collapse"
    :data-target="target"
    :aria-controls="target"
    :aria-expanded="toggled"
    aria-label="Toggle navigation"
  >
    <span class="navbar-toggler-icon"></span>
    <span class="navbar-toggler-icon"></span>
    <span class="navbar-toggler-icon"></span>
  </button>
</template>
<script>
export default {
  props: {
    target: {
      type: [String, Number],
      description: "Button target element"
    },
    toggled: {
      type: Boolean,
      default: false,
      description: "Whether button is toggled"
    }
  }
};
</script>
<style scoped>
.navbar-toggler-icon {
  width: 100%;
  height: 20px;
}
.navbar-toggler {
  width: 60px;
  height: 100%;
  line-height: 0.5;
  padding: 0.5rem 0.75rem;
  outline: none;
}
.navbar-light .navbar-toggler-icon {
  height: 4px;
  background: #019dd6 !important;
  border-radius: 2px;
}
</style>
