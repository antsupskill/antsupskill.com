<template>
  <div id="footer">
    <hr style="height:12px;color:##5d56c3;background-color:#5d56c3;margin:0" />
    <b-row no-gutters>
      <b-col class="my-3" md="6">
        <div class="mx-7rem">
          <router-link to="/">
            <b-img height="80px" :src="require('/src/assets/img/logo.png')"></b-img>
          </router-link>
          <br />
          <h4>Determination, Dedication & Discipline</h4>
        </div>
      </b-col>
      <b-col class="my-3" md="6">
        <div class="mx-7rem">
          <h5>
            © Copyright 2021 | Ants Skills Upgrade Solutions
            <br />All
            rights reserved.
          </h5>
          <h5>
            Connect with us on:
            <br />
            <div>
              <router-link class="fa-icons-spl" to="/social/twitter">
                <i class="fab fa-twitter fa-lg p-2"></i>
              </router-link>
              <router-link class="fa-icons-spl" to="/social/facebook">
                <i class="fab fa-facebook fa-lg p-2"></i>
              </router-link>
              <router-link class="fa-icons-spl" to="/social/instagram">
                <i class="fab fa-instagram fa-lg p-2"></i>
              </router-link>
            </div>
          </h5>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

<style scoped>
@media (min-width: 769px) {
  .mx-7rem {
    margin-left: 7rem;
    margin-right: 7rem;
  }
}
@media (max-width: 768px) {
  .mx-7rem {
    margin-left: 1rem;
    margin-right: 1rem;
  }
}
.fa-icons-spl {
  color: #256fb4;
}
.fa-icons-spl:hover {
  color: #358fd4;
}
</style>
