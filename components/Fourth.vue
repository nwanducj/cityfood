<template>
  <section class="d">
    <div class="text-center text__title my-4">Our Vendors</div>
    <v-row class="my-4">
      <v-col cols="12" sm="6" md="6" lg="6" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~assets/img/shopping.png" alt="" />
          </div>
          <div class="px-4">
            <div class="d-flex justify-space-between my-2">
              <div class="card__name">ShopRite</div>
              <v-rating
                v-model="value"
                dense
                size="18"
                color="secondary"
                readonly
              ></v-rating>
            </div>
            <div class="card__location d-flex align-items my-2">
              <v-icon size="18" color="black">mdi-map-marker-outline</v-icon>5,
              Independence Layout Enugu
            </div>
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6" md="6" lg="6" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~assets/img/shawarma.png" alt="" />
          </div>
          <div class="px-4">
            <div class="d-flex justify-space-between my-2">
              <div class="card__name">Handes Kitchen</div>
              <v-rating
                v-model="value"
                dense
                size="18"
                readonly
                color="secondary"
              ></v-rating>
            </div>
            <div class="card__location d-flex align-items my-2">
              <v-icon size="18" color="black">mdi-map-marker-outline</v-icon>5,
              Independence Layout Enugu
            </div>
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6" md="6" lg="6" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~assets/img/food.png" alt="" />
          </div>
          <div class="px-4">
            <div class="d-flex justify-space-between my-2">
              <div class="card__name">Licks & Chops</div>
              <v-rating
                v-model="value"
                dense
                size="18"
                readonly
                color="secondary"
              ></v-rating>
            </div>
            <div class="card__location d-flex align-items my-2">
              <v-icon size="16" color="black">mdi-map-marker-outline</v-icon>5,
              Independence Layout Enugu
            </div>
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6" md="6" lg="6" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~assets/img/egusi.png" alt="" />
          </div>
          <div class="px-4">
            <div class="d-flex justify-space-between my-2">
              <div class="card__name">Kilimanjaro</div>
              <v-rating
                v-model="value"
                dense
                size="18"
                readonly
                color="secondary"
              ></v-rating>
            </div>
            <div class="card__location d-flex align-items my-2">
              <v-icon size="18" color="black">mdi-map-marker-outline</v-icon>5,
              Independence Layout Enugu
            </div>
          </div>
        </div>
      </v-col>
    </v-row>
  </section>
</template>
<script>
export default {
  name: "fourth",
  data() {
    return {
      value: 4,
    };
  },
};
</script>
<style lang="scss" scoped>
.d {
  padding: 40px 20px 0 20px;
  width: 90%;
  margin: 0 auto;
}
img {
  width: 100%;
  height: 180px;
}
.card {
  width: 90%;
  height: 256px;
  background-color: #f8765a17;
  border-radius: 10px;
  &__location {
    font-size: 0.8rem;
  }
}
.text__title {
  font-size: 2rem;
  color: $secondary;
  font-weight: bold;
}
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .d {
    padding: 40px 20px;
    width: 90%;
    margin: 0 auto;
  }
}
@media only screen and (min-width: 992px) {
  .d {
    padding: 40px 20px;
    width: 80%;
    margin: 0 auto;
  }
}
</style>