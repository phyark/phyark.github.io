<script setup lang="ts">
import { ref } from 'vue';

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
	<h1>{{ msg }}</h1>
</template>

<style>
h1 {
	color: #ffffff;
  font-family: fantasy, Arial, "Helvetica Neue", Helvetica, sans-serif;
}
</style>
