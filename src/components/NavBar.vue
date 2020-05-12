<template>
  <nav
    class="nav w-screen z-20 text-blue"
    :class="ishome ? '' : 'shadow-2xl bg-green-800'"
  >
    <div class="left">
      <span class="font-light text-3xl">
        B-FRANCO
        <span class="font-semibold">Portfolio</span>
      </span>
    </div>
    <div class="right">
      <router-link class="link" to="/">Home</router-link>
      <router-link class="link" to="/portfolio">Portfolio</router-link>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    ishome: {
      type: Boolean,
      default: true
    }
  }
}
</script>

<style lang="scss" scoped>
.nav {
  @apply h-24;
}
.link {
  @apply px-2;
  &:hover {
    @apply text-yellow-500;
  }
}
</style>
