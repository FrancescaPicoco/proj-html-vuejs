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
        <p>THIS IS WHAT WE DO</p>
    </div>
    <div id="cardWrapper">
        <AppCard v-for="azioni in store.actionsCard" :details="azioni"/>
    </div>
</template>

<style scoped>
.topActions{
    padding: 3em 3rem 0 3rem;
    text-align: center;
}
p{
    margin-top: 2rem;
    font-size: 60px;
    font-weight: bold;
}
#cardWrapper{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}
</style>