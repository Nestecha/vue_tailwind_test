<template>
    <input class="base-text-input"
           type="text"
           :placeholder="placeholder"/>
</template>

<style lang="scss">
.base-text-input {
    @apply bg-white shadow rounded-lg border-none w-80 max-w-full leading-10 px-4;

    &:focus {
        @apply outline-none border-blue-200;
    }
}
</style>

<script>

export default {
    name: 'BaseTextInput',
    props: {
        placeholder: String,
    },
    data() {
        return {
            text: ''
        }
    },
}
</script>