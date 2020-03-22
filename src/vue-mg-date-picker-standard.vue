<template>
    <datepicker
        :input-class="{ 'is-invalid': isInvalid }"
        :language="ja" v-model="date"
        :format="format"
        :bootstrap-styling="true"
        ref="date"
        :calendarButton="calendarButton"
        calendarButtonIcon="far fa-calendar-alt"
        :clearButton="clearButton"
        clearButtonIcon="fas fa-times"
        style="width:11.5rem;"
        :typeable="typeable"
        :id="id"
    >
    </datepicker>
</template>

<script>
import moment from 'moment';
import Datepicker from 'vuejs-datepicker';
import {ja} from 'vuejs-datepicker/dist/locale'
export default {
    props: {
        value: '',
        format: {
            default: 'yyyy/MM/dd',
        },
        calendarButton: {
            default: true,
        },
        clearButton: {
            default: true,
        },
        typeable: {
            default: true,
        },
        id: '',
        isInvalid: '',
    },
    data () {
        return {
            date: '',
            ja: ja,
        }
    },
    mounted: function () {
        this.date = this.value
    },
    watch: {
        value: function () {
            this.date = this.value
        },
        date: function (val) {
            let d = val
            if (d) {
                d = moment(d).format('YYYY-MM-DD')
            }
            this.$emit('input', d)
        },
    },
    methods: {
    },
    components: {
        Datepicker
    }
}
</script>

<style lang="scss">
.vdp-datepicker .form-control:disabled,.vdp-datepicker .form-control[readonly] {
    background-color: white !important;
    // opacity: 1;
}
</style>
