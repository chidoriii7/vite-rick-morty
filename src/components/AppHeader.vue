<script>

import HeaderNav from './HeaderNav.vue';

export default {
    name: 'AppHeader',
    components: {
        HeaderNav,
    },

    data() {
        return {
            title: 'Rick and Morty App'
        }
    }
};
</script>

<template>
    <h1> {{ title }} </h1>
    <HeaderNav/>
</template>

<style>

</style>