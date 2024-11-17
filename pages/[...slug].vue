<!-- /pages/[...slug].vue -->
<script setup>
const route = useRoute();


const page = ref(route.fullPath);
</script>

<template>
    <h1>404 Not Found</h1>
    <p>你所請求的頁面：{{ page }}，不存在。</p>
    <NuxtLink class="btn btn-primary" to="/">返回首頁</NuxtLink>
</template>

<style scoped>
h1 {
    color: red;
    text-align: center;
}
p {
    text-align: center;
}
</style>