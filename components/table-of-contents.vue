<template>
    <div class="w-full h-8 bg-primary">
        <h1>Table of Contents</h1>
    </div>
    <ol class="list-decimal ml-4">
        <li v-for="system in systems" class="font-semibold text-md mt-2">
            <a :href="`#${system.id}`" class="toc-item block w-full">{{ system.name }}</a>
        </li>
    </ol>
</template>

<script lang="ts" setup>
defineProps<{ systems: { id: number, name: string }[] }>()
</script>

<style scoped>
.toc-item::after {
    content: target-counter(attr(href url), page)
}
</style>