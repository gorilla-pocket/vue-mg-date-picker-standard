<template>
  <section class="container">
    <date-picker-standard v-model="date"/>
  </section>
</template>

<style lang="scss" scoped>
</style>

<script>
import DatePickerStandard from '../src/vue-mg-date-picker-standard'
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
    DatePickerStandard,
  },  
}
</script>