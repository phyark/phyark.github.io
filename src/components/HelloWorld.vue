<script setup lang="ts">
defineProps<{ msg: string }>();
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
