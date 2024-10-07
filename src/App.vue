<template>
    <div class="container">
        <header-component></header-component>
    </div>
</template>

<style lang="scss" scoped>
@import './assets/scss/variables';
@import './assets/scss/mixins';

.container {
    width: 100%;
    height: 1000vh;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    background: $primary-bg-clr;

}
</style>

<script>
import Header from './components/Header.vue'
export default {
    components: {
        "header-component": Header,
    }
}
</script>
