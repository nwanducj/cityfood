<template>
  <div>
    <v-app-bar color="white" fixed app>
      <div class="d-flex align-center ml-sm-16">
        <img class="icon" src="~assets/img/cityfoodpng 1.png" />
        <img class="cityfood" src="~assets/img/cityfoodpng 2.png" />
      </div>
      <div
        class="d-none d-sm-flex text-center justify-center"
        style="width: 80%"
      >
        <div class="mx-8">About</div>
        <div class="mx-8">Contact</div>
        <div class="mx-8">Partnership</div>
      </div>
      <v-spacer class="d-sm-none"></v-spacer>
      <v-btn icon class="d-sm-none mr-2" @click="drawer = !drawer"
        ><v-icon size="30">mdi-menu</v-icon></v-btn
      >
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" absolute temporary>
      <div class="nav__item">
        <div class="py-4">
          <img class="icon" src="~assets/img/cityfoodpng 1.png" />
          <img class="cityfood" src="~assets/img/cityfoodpng 2.png" />
        </div>
        <div class="nav__text">About</div>
        <div class="nav__text">Contact</div>
        <div class="nav__text">Partnership</div>
      </div>
    </v-navigation-drawer>
    <First />
    <Second />
    <Third />
    <Fourth />
    <Fifth />
    <Sixth />
    <footer>
      <div class="footer mx-auto pa-8">
        <v-row>
          <v-col cols="6" sm="4">
            <div>
              <div class="title">Resources</div>
              <div>Privacy policy</div>
              <div>Terms of service</div>
            </div>
          </v-col>
          <v-col cols="6" sm="4">
            <div>
              <div class="title">Discover</div>
              <div>For Vendors</div>
              <div>Partnerships</div>
            </div>
          </v-col>
          <v-col cols="6" sm="4">
            <div>
              <div class="title">Follow us</div>
              <div class="d-flex align-items">
                <v-icon color="white" size="18" class="mr-2"
                  >mdi-facebook</v-icon
                >Facebook
              </div>
              <div>
                <v-icon color="white" size="18" class="mr-2">mdi-twitter</v-icon
                >Twitter
              </div>
              <div>
                <v-icon color="white" size="18" class="mr-2"
                  >mdi-linkedin</v-icon
                >LinkedIn
              </div>
              <div>
                <v-icon color="white" size="18" class="mr-2"
                  >mdi-instagram</v-icon
                >Instagram
              </div>
            </div>
          </v-col>
        </v-row>
      </div>
      <div class="text-center py-8">CityFood Copyright © 2020</div>
    </footer>
  </div>
</template>
<script>
export default {
  name: "index",
  data() {
    return {
      drawer: false,
    };
  },
  head() {
    return {
      title: "The Food is for the City",
      meta: [
        {
          hid: "description",
          name: "description",
          content:
            "Our job is to satisfy you with delicious meals from your favourite restaurants nearby, without moving an inch from your sofa, office, school or even bus station. Order Now!",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.full {
  height: 100vh;
}
.icon {
  height: 41px;
  width: 70px;
}
.cityfood {
  height: 22px;
  width: 70px;
}
.nav__item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
footer {
  background-color: lighten(black, 53%);
  color: white;
  .title {
    font-weight: 600;
    color: white;
  }
}
.nav__text {
  font-size: 1.4rem;
  padding: 10px 0;
}
.nav__text:hover {
  color: red;
}
@media only screen and (min-width: 600px) and (max-width: 960px) {
  .full {
    height: 100vh;
  }
}
@media only screen and (min-width: 960px) {
  .footer {
    width: 80%;
  }
  .full {
    height: 100vh;
  }
}
</style>