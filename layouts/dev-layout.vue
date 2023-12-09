<template>
    <div class="w-screen bg-gray-700 h-screen">
        <div class="pdf-container min-h-screen bg-white shadow-2xl">
            <PrintLayout>
                <slot/>
            </PrintLayout>
        </div>
    </div>
</template>

<script lang="ts" setup>
import PrintLayout from '~/layouts/print-layout.vue';
</script>

<style scoped>
.pdf-container {
    @apply container;
    width: 800px;
    max-width: 800px;
    min-width: 800px;
}
</style>