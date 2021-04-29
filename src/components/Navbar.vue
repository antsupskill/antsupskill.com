<template>
	<div>
		<b-navbar type="ants-blue" variant="faded">
			<b-navbar-nav>
				<b-navbar-brand to="/">
					<b-img
						height="70px"
						:src="require('/src/assets/img/logo.png')"
					></b-img>
				</b-navbar-brand>
			</b-navbar-nav>
			<b-navbar-nav class="ml-auto h5 text-ants-blue">
				<b-nav-item class="p-3" to="/">Home</b-nav-item>
				<b-nav-item class="p-3" to="/team">Team</b-nav-item>
				<b-nav-item class="p-3" to="/vision">Vision</b-nav-item>
				<b-nav-item class="p-3" to="/ceo-message"
					>CEO Message</b-nav-item
				>
				<b-nav-item class="p-3" to="/courses">Courses</b-nav-item>
				<b-nav-item class="p-3" to="/contact">Contact Us</b-nav-item>
			</b-navbar-nav>
		</b-navbar>
	</div>
</template>

<style scoped>
.navbar-ants-blue {
	background-color: white;
}
/* changing brand text color*/
.navbar-ants-blue .navbar-brand,
.navbar-ants-blue .navbar-text {
	color: #256fb4;
}
/* navigation link text color */
.navbar-ants-blue .navbar-nav .nav-link {
	color: #256fb4;
}
/* navigation links anchor hover and active styles */
.navbar-ants-blue .nav-item.active .nav-link,
.navbar-ants-blue .nav-item:hover .nav-link {
	color: #358fd4;
}
.navbar-ants-blue .navbar-nav .nav-link::after {
	color: #358fd4;
	content: '';
	display: block;
	width: 0;
	height: 3px;
	background: #358fd4;
	transition: width 0.3s;
}
.navbar-ants-blue .nav-item.active .nav-link::after,
.navbar-ants-blue .nav-item:hover .nav-link::after {
	color: #358fd4;
	width: 100%;
}
</style>
