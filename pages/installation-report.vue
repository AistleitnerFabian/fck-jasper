<template>
    <ProjectDetails/>
    <br>
    <p>this is an example <b>installation</b> report</p>
    <br>
    <TableOfContents :systems="systems"/>
    <br>
    <System v-for="system in systems" :system-id="system.id" :system-name="system.name"/>
</template>

<script lang="ts" setup>
const systems = [
    {id: 1, name: "AIO Seilsystem"},
    {id: 2, name: "Taurus Schienensystem"}
]
</script>

<style scoped>

</style>