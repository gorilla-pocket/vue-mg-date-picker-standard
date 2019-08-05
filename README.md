# vue-mg-date-picker-normal

## Installation

```
npm i vue-mg-date-picker-normal
```

## Usage

app.js

```
import DatePickerNormal from 'vue-mg-date-picker-normal'
Vue.component('DatePickerNormal', DatePickerNormal)
```

Example:

```
<template>
    <section class="container">
        <date-picker-normal v-model="date"/>
    </section>
</template>

<script>
export default {
    data() {
        return {
            date: '',
        }
    },
}
</script>
```

## License

MIT