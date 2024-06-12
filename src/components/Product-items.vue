<template>
    <div>
        <p v-if="isAvailable">Show Products</p>
        <p v-else-if="isAvailable && count < 5">Running low of stock</p>
        <p v-else>Sold Out!</p>
    </div>
</template>

<script>
export default {
    name: 'Products',
    data() {
        return {
            isAvailable: true,
            count: 3,
        };
    },
    methods: {
        incrementCount() {
            this.count++;
        },
    },
    mounted() {
        console.log('mounted has been invoked');
    },
};
</script>

<style scoped>
/* Your component-specific styles go here */
</style>