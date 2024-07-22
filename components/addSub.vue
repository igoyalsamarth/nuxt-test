<script setup>
const number = useState("number", () => 0)
const show = useState('show', () => false)
</script>

<template>
    <div>
        <p>number: {{ number }}</p>
        <p>show : {{ show }}</p>
        <button @click="number++">Add</button>
        <button @click="number--">Minus</button>
        <button @click="show = !show">Show</button>
        <HideShow :show="show" />
    </div>
</template>