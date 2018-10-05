<template>
    <transition name="fade-down">
        <slot/>
    </transition>
</template>

<script>
    export default {
        name: 'transition-fade-down',
    };
</script>

<style lang="scss">
    .fade-down-enter-active,
    .fade-down-leave-active {
        transition: 0.2s ease;
    }
    .fade-down-enter,
    .fade-down-leave-to {
        opacity: 0;
    }
    .fade-down-leave-to {
        transform: translateY(10px);
    }
    .fade-down-enter {
        transform: translateY(-10px);
    }
</style>