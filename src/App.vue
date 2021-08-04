<template>
  <div class="container">
    <Human />
    <Human />
    <Human />
    <Human />
    <Human />
  </div>
</template>

<script>
import Human from "@/components/Human.vue"
export default {
  components: {
    Human,
  },
}
</script>

<style scoped>
.container {
  display: flex;
}
</style>