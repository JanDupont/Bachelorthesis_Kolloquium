---
layout: two-cols-header
clicks: 4
---

# Implementierung Frontend

::left::

<ul>
    <li v-if="$slidev.nav.clicks >= 1 "><strong>Vue SFC</strong></li><li v-else>Vue SFC</li>
    <li v-if="$slidev.nav.clicks >= 1 "><strong>Vue Composition API</strong></li><li v-else>Vue Composition API</li>
</ul>

<style>
    strong {
        color: lightgreen !important;
    }
</style>

::right::
<v-clicks>

```ts {all|1|3-13|14}
<template></template>

<script setup lang="ts">
import { defineProps, PropType } from "vue";
const props = defineProps({
	emoji: {
		type: String as PropType<string | number>,
		default: "",
		required: true,
	},
});
</script>

<style scoped lang="scss"></style>
```

</v-clicks>
