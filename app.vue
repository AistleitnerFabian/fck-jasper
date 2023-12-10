<template>
    <NuxtLayout :name="layoutName">
        <NuxtPage/>
    </NuxtLayout>
</template>

<script lang="ts" setup>
const devMode: boolean = useRoute().query.dev === "true"
const layoutName = ref(!devMode ? 'print-layout' : "dev-layout")
</script>

<style>
</style>