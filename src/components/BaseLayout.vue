<template>

    <BaseHeader />

        <div class="main-content">

            <slot></slot>

        </div>
        
    <BaseFooter />

</template>

<script>

    import BaseFooter from './BaseFooter.vue'
    import BaseHeader from './BaseHeader.vue'

    export default {
    name: 'BaseLayout',
    components: {
        BaseHeader,
        BaseFooter
    }

    }
</script>

<style>

    .main-content {
    flex: 1;
    padding: 20px;
    }

</style>