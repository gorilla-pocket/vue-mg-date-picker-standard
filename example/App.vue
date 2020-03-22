<template>
  <section class="container">
    <date-picker-standard style="width:11rem;" v-model="date"/>
    <date-picker-standard v-model="date"/>
  </section>
</template>

<style lang="scss" scoped>
</style>

<script>
import DatePickerStandard from '../src/vue-mg-date-picker-standard'
import 'bootstrap/dist/css/bootstrap.min.css'
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