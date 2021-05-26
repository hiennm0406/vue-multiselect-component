# Multiselect component for Vue 2

## Install & basic usage
![img.png](docs/img.png)
```shell
$ npm install vue-multiselect-component
```

```vue
<template>
  <VueMultiselectComponent
    v-model="selected"
  />
</template>

<script>
import VueMultiselectComponent from 'vue-multiselect-component'

export default {
  components: {
    VueMultiselectComponent
  },
  data() {
    return {
      selected: [],
      options: [
        { id: 'ru', label: 'Russia' },
        { id: 'nl', label: 'Netherlands' },
        { id: 'fr', label: 'France' }
      ]
    }
  }
}
</script>
```

## Props

|Props|Description|Required|Type|Default|
|-----|-----------|--------|----|-------|
|value (v-model)|Selected items|true|Array|-|
|options|List of all items|true|Array|-|
|writable|The ability to write in the input field|false|Boolean|true|
|searchable|Standard element search (only for writable = true)|false|Boolean|true|
|placeholder|Input placeholder|false|String|-|
|loading|Options list standby mode|false|Boolean|false|

**will be complemented*

## Events
|Event|Description|Attributes|
|-----|-----------|-----|
|search-change|Emitted after the search query changes|(search-query)

**will be complemented*

## License

Copyright (c) 2021-present [Anatoliy Vasilyev](https://github.com/vas11yev1work).

Released under the [MIT License](https://github.com/vas11yev1work/vue-multiselect-component/blob/main/LICENSE).
