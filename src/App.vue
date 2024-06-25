<template>
    <div id="app">
        <page-header></page-header>

        <div class="container">
            <offer-list/>
        </div>
    </div>
</template>

<style lang="scss">
html, body {
    @apply font-sans p-0 m-0 bg-gray-50;

    .container {
        @apply max-w-screen-xl mx-auto px-2;
    }

    .base-button {
        @apply bg-blue-400 rounded w-full border-none p-2 text-white focus:outline-none uppercase cursor-pointer;

        &-disabled {
            @apply bg-gray-200 cursor-not-allowed;
        }
    }
}
</style>


<script>
import PageHeader from "@/components/layout/PageHeader.vue";
import OfferList from "@/components/offers/OfferList.vue";

export default {
    name: 'App',
    components: {
        OfferList,
        PageHeader
    }
}
</script>