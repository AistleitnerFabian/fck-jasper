<template>
    <table class="w-full">
        <thead>
        <tr>
            <th>
                <DocumentHeader/>
            </th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>
                <div class="p-8">
                    <slot/>
                </div>
            </td>
        </tr>
        </tbody>
        <tfoot>
        <tr>
            <td>
                <div class="h-20">
                    <!-- this must be the same height as the footer -->
                </div>
            </td>
        </tr>
        </tfoot>
    </table>

    <div class="print:fixed print:bottom-0 w-full">
        <DocumentFooter/>
    </div>
</template>

<script lang="ts" setup>
</script>

<style scoped>

thead {
    display: table-header-group;
}

tfoot {
    display: table-footer-group;
}
</style>