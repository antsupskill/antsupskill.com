<template>
  <div>
    <b-navbar toggleable="lg" type="ants-blue" variant="faded">
      <b-navbar-brand to="/">
        <b-img height="70px" :src="require('/src/assets/img/logo.png')"></b-img>
      </b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto h5 text-ants-blue">
          <b-nav-item class="p-3" to="/">Home</b-nav-item>
          <b-nav-item class="p-3" to="/team">Team</b-nav-item>
          <b-nav-item class="p-3" to="/vision">Vision</b-nav-item>
          <b-nav-item class="p-3" to="/ceo-message">CEO Message</b-nav-item>
          <b-nav-item class="p-3" to="/courses">Courses</b-nav-item>
          <b-nav-item class="p-3" to="/contact">Contact Us</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<style scoped>
.navbar-ants-blue .navbar-toggler-icon {
  background-image: url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 32 32' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath stroke='rgba(255,102,203, 0.5)' stroke-width='2' stroke-linecap='round' stroke-miterlimit='10' d='M4 8h24M4 16h24M4 24h24'/%3E%3C/svg%3E");
}
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
  content: "";
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
