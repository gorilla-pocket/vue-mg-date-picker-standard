<template>
  <section class="container">
    <date-picker-normal v-model="date"/>
  </section>
</template>

<style lang="scss" scoped>
</style>

<script>
import DatePickerNormal from '../src/vue-mg-date-picker-normal'
export default {
  data() {
    return {
      date: '',
    }
  },
    methods: {
      ///
    },
  components: {
    DatePickerNormal,
  },  
}
</script>