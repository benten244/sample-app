<template>
  <div class="human-cloth" v-bind:class="clothType">
      <slot />
  </div>
</template>

<script>
export default {
    props: {
      clothType:{
        validator(value){
          return["👗", "👔", "👕"].includes(value)
        }
      },
    },
}
</script>


<style>

</style>