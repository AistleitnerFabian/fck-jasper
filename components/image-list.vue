<template>
    <div class="w-full h-8 bg-primary">
        <h1>Images</h1>
    </div>
    <div class="grid grid-cols-2 gap-2 pt-2">
        <div v-for="img in images">
            <img :src="img" alt="test image" class="w-full"/>
        </div>
    </div>
</template>

<script lang="ts" setup>
const imageUrl = "https://picsum.photos/1920/1080"
const images = []
for (let i = 0; i < 5; i++) {
    images.push(`${imageUrl}?i=${i}`)
}
</script>

<style scoped>

</style>