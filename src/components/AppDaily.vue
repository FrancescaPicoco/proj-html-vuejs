<script>
import { store } from "../store.js"
import AppCard3 from "./AppCard4.vue"
export default {
    name : "AppDaily",
	components: {
    AppCard3
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
        <AppCard4 v-for="day in store.dailyCard" :details3="day"/>
    </div>
</template>

<style scoped>
.cardWrapper{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    height: 70vh;
    background-color: cadetblue;
}
</style>