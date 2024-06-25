<template>
    <div class="page-header">
        <div class="container">
            <img :src="require('@/assets/images/logo.svg')" alt="Kang"/>
        </div>
    </div>
</template>

<style lang="scss">
.page-header {
    @apply bg-gray-700 h-16;

    .container {
        @apply h-16;
    }

    img {
        @apply h-14 my-1;
    }
}
</style>

<script>
export default {
    name: 'PageHeader',
}
</script>