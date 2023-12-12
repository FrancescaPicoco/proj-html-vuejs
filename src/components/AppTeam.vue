<script>
import { store } from "../store.js"
import AppCard3 from "./AppCard3.vue"
export default {
    name : "AppTeam",
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
        <AppCard3 v-for="member in store.teamCard" :details3="member"/>
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