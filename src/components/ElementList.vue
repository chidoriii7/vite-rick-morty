<script>
 import { store } from '../store'
export default {
    name: 'ElementList',
    data(){
        return{
            store
        }
    }
}
</script>

<template>
    <div>
        <ul>
            <li v-for="card in store.results">
            <div> {{card.name}} </div>
            <img :src="card.image" alt="">
            </li>
        </ul>
    </div>
</template>

<style>

</style>