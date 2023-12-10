<template>
    <div class="break-before-page">
        <div :id="systemId" class="w-full h-8 bg-primary">
            <h1>System: {{ systemName }}</h1>
        </div>
        <p>System should always be on a new Page</p>
        <br>
        <ImageList/>
        <br>
    </div>
</template>

<script lang="ts" setup>
defineProps<{ systemName: string, systemId: number }>()
</script>

<style scoped>

</style>