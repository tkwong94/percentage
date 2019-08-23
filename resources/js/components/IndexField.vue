<template>
  <span v-if="field.value == null">—</span>
  <span v-else>{{ field.value.toFixed(field.precision) }}%</span>
</template>

<script>
export default {
  props: ["resourceName", "field"]
};
</script>
