<template>
  <div>
    <div class="d-flex py-4 align-center heading">
      <div class="d-flex align-center ml-sm-16">
        <img class="icon" src="~assets/img/cityfoodpng 1.png" />
        <img class="cityfood" src="~assets/img/cityfoodpng 2.png" />
      </div>
      <div
        class="d-none d-sm-flex text-center justify-center"
        style="width: 80%"
      >
        <div class="mx-8" @click="gotoThird">About</div>
        <div class="mx-8" @click="gotoFourth">Vendors</div>
        <div class="mx-8" @click="gotoSixth">Partnership</div>
        <v-btn class="mx-8 text-none" color="primary" @click="gotoSixth"
          >Contact</v-btn
        >
      </div>
      <v-spacer class="d-sm-none"></v-spacer>
      <v-btn icon class="d-sm-none mr-2" @click="drawer = !drawer"
        ><v-icon size="30">mdi-menu</v-icon></v-btn
      >
    </div>
    <v-navigation-drawer v-model="drawer" fixed temporary>
      <div class="nav__item">
        <div class="py-4">
          <img class="icon" src="~assets/img/cityfoodpng 1.png" />
          <img class="cityfood" src="~assets/img/cityfoodpng 2.png" />
        </div>
      </div>
      <v-list nav dense>
        <v-list-item-group active-class="primary--text text--primary-4">
          <v-list-item>
            <v-list-item-title @click="gotoThird">About</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title @click="gotoSixth">Contact</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title @click="gotoSixth"
              >Partnership</v-list-item-title
            >
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    <First />
    <Second />
    <Third id="myRef3" />
    <Fourth id="myRef4" />
    <Fifth />
    <Sixth id="myRef" />
    <Footer
      :gotoSixth="gotoSixth"
      :gotoThird="gotoThird"
      :gotoFourth="gotoFourth"
    />
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
    gotoSixth() {
      document.getElementById("myRef").scrollIntoView();
      this.drawer = false;
    },
    gotoThird() {
      document.getElementById("myRef3").scrollIntoView();
      this.drawer = false;
    },
    gotoFourth() {
      document.getElementById("myRef4").scrollIntoView();
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
.heading {
  background-color: white;
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 100;
  box-shadow: 1px 2px 4px #aaaaaa;
}
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