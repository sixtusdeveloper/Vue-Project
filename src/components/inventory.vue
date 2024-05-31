<template>
    <div>
        <p v-if="available">Show Products</p>
        <p v-else>Sold Out!</p>
    </div>
</template>

<script>
export default {
    name: 'Inventory',
    data() {
        return {
            isAvailable: false,
        };
    },
    computed: {
        available() {
            return this.isAvailable;
        },
    },
};
</script>

<style scoped>
/* Your component-specific styles go here */
</style>