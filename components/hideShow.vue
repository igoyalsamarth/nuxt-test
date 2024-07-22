<script setup>
const props = defineProps({
    show: {
        type: Boolean,
    },
});
const show = props;
</script>

<template>
    <p>{{ show.show ? 'Show' : 'Hide' }}</p>
    <p v-if="show.show">Show</p>
    <p v-else>Hide</p>
</template>