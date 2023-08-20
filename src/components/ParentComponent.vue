<script setup>
import { ref } from 'vue';
import ChildComponent from './ChildComponent.vue';

const message = ref('Message from parent component');

const messageEmitted =ref('');
</script>

<template>
 <h1 class="text-xl font-bold text-orange-500">{{ messageEmitted  }}</h1> 

<div>
   <ChildComponent :message="message" v-model:messageEmitted ="messageEmitted"/>
 </div>
</template>

<style scoped>

</style>
