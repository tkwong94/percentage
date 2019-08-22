<template>
    <panel-item :field="field">
        <template slot="value">
            <div v-if="field.value == null">
                111—
            </div>
            <div v-else>
                111{{ field.value.toFixed(field.precision) }}%
            </div>
        </template>
    </panel-item>
</template>

<script>
    export default {
        props: ['resource', 'resourceName', 'resourceId', 'field'],
    }
</script>
