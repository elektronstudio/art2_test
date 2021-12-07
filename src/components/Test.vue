<script setup lang="ts">
let a = $ref(0);
</script>

<template><input type="range" v-model="a" />{{ a }}</template>
