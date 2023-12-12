<script>
import { store } from "./store.js" ;
import AppHeader from "./components/AppHeader.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import AppActions from "./components/AppActions.vue"
import AppJumbotron2 from "./components/AppJumbotron2.vue"
import AppWatchlist from "./components/AppWatchlist.vue"
import AppCounter from "./components/AppCounter.vue"
import AppTeam from "./components/AppTeam.vue"
import AppJumbotron3 from "./components/AppJumbotron3.vue"
import AppDaily from "./components/AppDaily.vue"
import AppLogo from"./components/AppLogo.vue"
import AppMail from "./components/AppMail.vue"
import AppFooter from "./components/AppFooter.vue"
export default {
	components: {
    AppHeader,
    AppJumbotron,
	AppActions,
	AppJumbotron2,
	AppWatchlist,
	AppCounter,
	AppTeam,
	AppJumbotron3,
	AppDaily,
	AppLogo,
	AppMail,
	AppFooter
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
  <AppCounter />
  <AppTeam />
  <AppJumbotron3 />
  <AppDaily />
  <AppLogo />
  <AppMail />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss';
</style>

<style scoped lang="scss">
// @use './styles/partials/variables' as *;

</style>
