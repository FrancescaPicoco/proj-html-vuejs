<script>
import { store } from "../store.js"
import AppCard2 from "./AppCard2.vue"
export default {
    name : "AppWatchlist",
	components: {
    AppCard2
	},
    data(){
        return{
            store
        }
    }
	
}
</script>

<template>
    <div class="topWatchlist">
        <span>YOUR WATCHLIST</span>
        <h1>BEST HITS MOVIE</h1>
    </div>
    <div class="cardWrapper">
        <AppCard2 v-for="film in store.watchlistCard" :details2="film"/>
    </div>
</template>

<style scoped>
.topWatchlist{
    padding: 3em;
    text-align: center;
}
h1{
    margin-top: 0;
    font-size: 50px;
}
.cardWrapper{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}
</style>