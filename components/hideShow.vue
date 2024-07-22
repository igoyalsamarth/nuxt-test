<script setup>
const props = defineProps({
    show: {
        type: Boolean,
    },
});
const show = props;
</script>

<template>
    <p v-if="show.show">Show</p>
    <p v-else>Hide</p>
</template>