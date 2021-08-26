<template>
  <div class="order-summary">
    <slot />
  </div>
</template>

<script>
export default {
  name: "Page"
}
</script>

<style lang="scss" scoped>
    .order-summary {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      width: 100%;
      height: 100%;
      background: #e0e8ff;

      &:before {
        content: '';
        position: fixed;
        inset: 0;
        width: 100%;
        height: 100%;
        background-image: url('../assets/background-desktop.svg');
        background-repeat: no-repeat;
        background-size: 100% auto;
        background-position: top center;
      }

      @media (max-width: 375px) {
        &:before {
          background-image: url('../assets/background-mobile.svg');
          background-size: auto;
        }
      }
    }
</style>
