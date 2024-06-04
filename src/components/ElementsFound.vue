
<script>
    import { store } from '../store'
    export default {
        name: 'ElementsFound',
        data(){
        return{
            store
        }
    }
    };
</script>

<template>
    <div> Found {{ store.info.count }} characters </div>
</template>