<template>
  <div class="container">
    <Human v-bind:cloth="clothes[0]"><Human /></Human>
    <Human v-bind:cloth="clothes[1]"><Human /></Human>
    <Human v-bind:cloth="clothes[2]"><Human /></Human>
 </div>
</template>

<script>
import Human from "@/components/Human.vue"
export default {
  components: {
    Human,
  },
  data(){
    return{
      clothes: [
        {id: 0, text: "👗"},
        {id: 1, text: "👔"},
        {id: 2, text: "🎽"},
      ],
    }
  },
}
</script>

<style scoped>
.container {
  display: flex;
}
</style>