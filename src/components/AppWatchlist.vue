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
    <div class="cardWrapper">
        <AppCard2 v-for="film in store.watchlistCard" :details2="film"/>
    </div>
</template>

<style scoped>
.cardWrapper{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}
</style>