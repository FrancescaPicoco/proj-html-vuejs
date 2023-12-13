<script>
import { store } from "../store.js"
import AppCard from "./AppCard.vue"
export default {
    name : "AppActions",
	components: {
    AppCard
	},
    data(){
        return{
            store
        }
    }	
}
</script>

<template>
    <div class="topActions">
        <span>PELICULA STUDIO</span>
        <h1>THIS IS WHAT WE DO</h1>
    </div>
    <div id="cardWrapper">
        <AppCard v-for="azioni in store.actionsCard" :details="azioni"/>
    </div>
</template>

<style scoped>
.topActions{
    padding: 3em;
    text-align: center;
}
h1{
    margin-top: 0;
    font-size: 60px;
}
#cardWrapper{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}
</style>