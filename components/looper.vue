<script setup>
const props = defineProps({
    data: {
        type: Object,
    },
},
);
const data = props;
</script>

<template>
    <div v-for="item in data.data">
        <p>{{ item.color }} - {{ item.value }}</p>
    </div>
</template>