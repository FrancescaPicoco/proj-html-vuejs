<script>
import { store } from "../store.js"
export default {
  name: "AppCard3",
    props: ["details3"],
	components: {
	},
	data() {
		return {
			store,
		}
  }
}
</script>

<template> 
    <div class="card">
      <div class="cardTop">
        <img :src=details3.teamSrc>
      </div>
      <div class="cardDescr">
        <h3>{{ details3.titolo }}</h3>
        <span>{{ details3.text }}</span>
      </div>
    </div>  
</template>
<style scoped>

.card{
 width: calc((100% / 4) - 4rem);
 margin: 2rem;
 background-color: slategray;
 color: black;
}
img{
 width: 100%;
 object-fit: contain;
}
</style>