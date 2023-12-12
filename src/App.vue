<script>
import { store } from "./store.js" //state management
import AppHeader from "./components/AppHeader.vue"
import AppJumbotron from "./components/AppJumbotron.vue"
import AppActions from "./components/AppActions.vue"
import AppJumbotron2 from "./components/AppJumbotron2.vue"
import AppWatchlist from "./components/AppWatchlist.vue"
export default {
	components: {
    AppHeader,
    AppJumbotron,
	AppActions,
	AppJumbotron2,
	AppWatchlist
	},
	data() {
		return {
			store,
		}
	}
}
</script>

<template>
  <AppHeader/>
  <AppJumbotron/>
  <AppActions/>
  <AppJumbotron2 />	
  <AppWatchlist />
</template>

<style lang="scss">
@use './styles/general.scss';
</style>

<style scoped lang="scss">
// @use './styles/partials/variables' as *;

</style>
