<template>
<main class="container">
    <AppHeader />
    <AppRestaurantInfo :datasource="fooddata" />
</main>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue';
export default {
    components: {
        AppHeader,
        AppRestaurantInfo
    },
    computed: {
        fooddata() {
            return this.$store.state.fooddata;
        },
    },
}
</script>

<style></style>
