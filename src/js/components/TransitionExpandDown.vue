<template>
    <transition name="expandDown">
        <slot/>
    </transition>
</template>

<script>
    export default {
        name: 'transition-expand-down',
    };
</script>

<style lang="scss">
    .expandDown-enter-active,
    .expandDown-leave-active {
        transition: all 0.5s;
        max-height: 999px;

    }
    .expandDown-enter,
    .expandDown-leave-to {
        opacity: 0;
        max-height: 0;

    }
</style>