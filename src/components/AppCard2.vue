<script>
import { store } from "../store.js"
export default {
  name: "AppCard2",
    props: ["details2"],
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
        <img :src="details2.watchSrc">
      </div>
      <div class="cardDescr">
        <h3>{{ details2.titolo }}</h3>
        <span>{{ details2.type }}</span>
      </div>
    </div>  
</template>
<style scoped>

.card{
 width: calc((100% / 3) - 5rem);
 margin: 2.5rem;
 color: black;
}
img{
    width: 100%;
}
.cardDescr{
    text-align: center;
}
span{
    color: slategrey;
}
</style>