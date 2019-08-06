# vue-mg-date-picker-standard

![npm](https://img.shields.io/npm/v/vue-mg-date-picker-standard)
![npm](https://img.shields.io/npm/dm/vue-mg-date-picker-standard)

## Installation

```
npm i vue-mg-date-picker-standard
```

## Usage

app.js

```
import DatePickerStandard from 'vue-mg-date-picker-standard'
Vue.component('DatePickerStandard', DatePickerStandard)
```

Example:

```
<template>
    <section class="container">
        <date-picker-standard v-model="date"/>
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
