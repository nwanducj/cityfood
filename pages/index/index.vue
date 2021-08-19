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
        <div class="mx-8" @click="gotoThird">About</div>
        <div class="mx-8" @click="gotoSixith">Contact</div>
        <div class="mx-8" @click="gotoSixith">Partnership</div>
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
        <div class="nav__text" @click="gotoThird">About</div>
        <div class="nav__text" @click="gotoSixith">Contact</div>
        <div class="nav__text" @click="gotoSixith">Partnership</div>
      </div>
    </v-navigation-drawer>
    <First />
    <Second />
    <Third id="myRef3" />
    <Fourth />
    <Fifth />
    <Sixth id="myRef" />
    <Footer />
  </div>
</template>
<script>
export default {
  name: "index",
  data() {
    return {
      drawer: false,
      myRef: "contact",
    };
  },
  methods: {
    gotoSixith() {
      document.getElementById("myRef").scrollIntoView();
      this.drawer = false;
    },
    gotoThird() {
      document.getElementById("myRef3").scrollIntoView();
      this.drawer = false;
    },
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
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .full {
    height: 100vh;
  }
}
@media only screen and (min-width: 992px) {
  .footer {
    width: 80%;
  }
  .full {
    height: 100vh;
  }
}
</style>