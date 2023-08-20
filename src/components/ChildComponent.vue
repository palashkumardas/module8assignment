<script setup>

    defineProps(['message','messageEmitted']);
    defineEmits(['update:messageEmitted']);

</script>

<template>
        <h3 class="text-xl font-bold text-gray-900">{{ message }}</h3>
        <!-- <h3 class="text-xl font-bold text-gray-900"> {{ messageEmitted }}</h3> -->
        <button class="bg-blue-500 text-white-400" @click="$emit('update:messageEmitted','Message from child component')">Click</button>
</template>

<style scoped>

</style>
