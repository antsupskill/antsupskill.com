<template>
	<div id="app" style="font-family:'Rajdhani',sans-serif">
		<Navbar></Navbar>
		<router-view />
		<Footer></Footer>
	</div>
</template>

<script>
import Navbar from '@/components/Navbar.vue';
import Footer from '@/components/Footer.vue';

export default {
	name: 'App',
	components: {
		Navbar,
		Footer
	}
};
</script>

<style lang="scss">
@import 'assets/scss/app.scss';
</style>

<style>
@import '../node_modules/@fortawesome/fontawesome-free/css/all.min.css';
</style>
