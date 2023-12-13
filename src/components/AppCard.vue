<script>
import { store } from "../store.js"
export default {
  name: "AppCard",
    props: ["details"],
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
        <img :src=details.actionsSrc>
      </div>
      <div class="cardDescr">
        <h3>{{ details.titolo }}</h3>
        <span>{{ details.text }}</span>
      </div>
    </div>  
</template>
<style scoped>

.card{
 width: calc((100% / 3) - 5rem);
 margin: 2.5rem;
 color: black;
}
.cardTop{
  display: flex;
  justify-content: center;
}
.cardDescr{
  text-align: center;
}
span{
  font-size: 18px;
  color: slategrey;
}
img{
 width: 20%;
 object-fit: contain;
}
</style>