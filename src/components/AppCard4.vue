<script>
import { store } from "../store.js"
export default {
  name: "AppCard4",
    props: ["details4"],
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
        <img :src=details4.dailySrc>
      </div>
      <div class="cardDescr">
        <h3>{{ details4.titolo }}</h3>
        <span>{{ details4.text }}</span>
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