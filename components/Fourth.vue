<template>
  <div>
    <div
      class="testimonial-area-l-13 position-relative overflow-hidden z-index-1"
    >
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-xl-11">
            <div class="row">
              <div class="col-md-12">
                <div class="section-heading-7 text-center">
                  <h2 class="secondary--text">Our Vendors</h2>
                </div>
              </div>
            </div>
            <div
              class="row testimonial-area-l-13-items justify-content-center"
              data-aos="fade-right"
              data-aos-duration="800"
              data-aos-once="true"
            >
              <div class="col-xl-4 col-md-6 col-sm-8">
                <div class="testimonial-card bg-white">
                  <div class="mb-n2">
                    <img src="~assets/img/shopping.png" alt="" />
                  </div>
                  <div class="pa-4" style="background-color: #f8765a1f">
                    <div
                      class="d-flex align-items-center justify-space-between"
                    >
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
                      <v-icon size="18" color="black"
                        >mdi-map-marker-outline</v-icon
                      >5, Independence Layout Enugu
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-xl-4 col-md-6 col-sm-8">
                <div class="testimonial-card bg-white">
                  <div class="mb-n2">
                    <img src="~assets/img/shawarma.png" alt="" />
                  </div>
                  <div class="pa-4" style="background-color: #f8765a1f">
                    <div
                      class="d-flex align-items-center justify-space-between"
                    >
                      <div class="card__name">Handes Kitchen</div>
                      <v-rating
                        v-model="value"
                        dense
                        size="18"
                        color="secondary"
                        readonly
                      ></v-rating>
                    </div>
                    <div class="card__location d-flex align-items my-2">
                      <v-icon size="18" color="black"
                        >mdi-map-marker-outline</v-icon
                      >5, Independence Layout Enugu
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-xl-4 col-md-6 col-sm-8">
                <div class="testimonial-card bg-white">
                  <div class="mb-n2">
                    <img src="~assets/img/food.png" alt="" />
                  </div>
                  <div class="pa-4" style="background-color: #f8765a1f">
                    <div
                      class="d-flex align-items-center justify-space-between"
                    >
                      <div class="card__name">Licks & Chops</div>
                      <v-rating
                        v-model="value"
                        dense
                        size="18"
                        color="secondary"
                        readonly
                      ></v-rating>
                    </div>
                    <div class="card__location d-flex align-items my-2">
                      <v-icon size="18" color="black"
                        >mdi-map-marker-outline</v-icon
                      >5, Independence Layout Enugu
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-xl-4 col-md-6 col-sm-8">
                <div class="testimonial-card bg-white">
                  <div class="mb-n2">
                    <img src="~assets/img/egusi.png" alt="" />
                  </div>
                  <div class="pa-4" style="background-color: #f8765a1f">
                    <div
                      class="d-flex align-items-center justify-space-between"
                    >
                      <div class="card__name">Kilimanjaro</div>
                      <v-rating
                        v-model="value"
                        dense
                        size="18"
                        color="secondary"
                        readonly
                      ></v-rating>
                    </div>
                    <div class="card__location d-flex align-items my-2">
                      <v-icon size="18" color="black"
                        >mdi-map-marker-outline</v-icon
                      >5, Independence Layout Enugu
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- <div class="bg-shape-3"></div> -->
    </div>
  </div>
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
// img {
//   width: 100%;
//   height: 180px;
// }
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