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
    <div class="topTeam">
        <span>THE PERICUROS</span>
        <p>MEET THE TEAM</p>
    </div>
    <div class="cardWrapper">
        <AppCard3 v-for="member in store.teamCard" :details3="member"/>
    </div>
</template>

<style scoped>
.topTeam{
    text-align: center;
    margin-top: 3rem;
}
p{
    margin-top: 0.3rem;
    font-size: 50px;
}
.cardWrapper{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    padding: 0 2rem 2rem 2rem;
}
</style>