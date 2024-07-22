<script setup>

const {data:products, status} = await useLazyFetch('/api/products');
</script>

<template>
    <div>
        <p v-if="status === 'pending'">Loading</p>
        <Looper v-else :data="products" />
    </div>
</template>