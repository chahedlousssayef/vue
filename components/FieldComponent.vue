<script setup lang="ts">
    interface FieldComponentProperties {
        id: string;
        type?: string;
        label: string;
        placeholder: string;
    }

    defineProps<FieldComponentProperties>();
</script>

<template>
    <section>
        <label :for="id">{{label}}</label>
        <input :type="type ?? 'text'" :id="id" :name="id" :placeholder="placeholder">
   </section>
</template>

<style scoped>
</style>