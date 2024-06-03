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
    <div> {{ title }} </div>
    <HeaderNav/>
</template>

<style>

</style>