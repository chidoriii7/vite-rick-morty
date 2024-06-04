<script>
  import axios from 'axios';
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import { store } from './store';

  export default {
    nome: 'vite-rick-morty',
    components: {
      AppHeader,
      AppMain,
    },
    data(){
      return {
        store,
      }
    },
    created(){
      axios.get(this.store.apiUrl).then((response) => {
        this.store.info = response.data.info;
        console.log(response.data.info)
        this.store.results = response.data.results
        console.log(response.data.results)

      })
    }
  };
</script>

<template>

  <AppHeader/>
  <AppMain/>
  

</template>

<style>

</style>
