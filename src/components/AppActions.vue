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
    <div id="cardWrapper">
        <AppCard v-for="azioni in store.actionsCard" :details="azioni"/>
    </div>
</template>

<style scoped>
#cardWrapper{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}
</style>