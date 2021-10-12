<template>
  <section class="b mx-auto mt-8">
    <div class="row">
      <div class="col-md-12">
        <div class="section-heading-7 text-center">
          <h2 class="black--text">How to Order</h2>
        </div>
      </div>
    </div>
    <v-row justify="center">
      <v-col cols="12" sm="6" md="4" lg="4" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~/assets/img/order (1).png" />
          </div>
          <div class="card__title">Download City Food App</div>
          <div class="card__text">
            Download App on Apple or google play store
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="4" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~/assets/img/order (2).png" />
          </div>
          <div class="card__title">Set Delivery Location</div>
          <div class="card__text">
            Select the location where you want us to deliver
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="4" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~/assets/img/order (3).png" />
          </div>
          <div class="card__title">Choose a Resturant Near you</div>
          <div class="card__text">
            Select your favorite restaurant or search food
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="4" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~/assets/img/order (4).png" />
          </div>
          <div class="card__title">Select food of your choice</div>
          <div class="card__text">
            Select food by adding it to cart and making payment.
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="4" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~/assets/img/order (5).png" />
          </div>
          <div class="card__title">Receive food at your doorstep</div>
          <div class="card__text">
            Your order will be delivered to you in no time.
          </div>
        </div>
      </v-col>
      <v-col cols="12" sm="6" md="4" lg="4" align="center" justify="center">
        <div class="card">
          <div class="card__photo">
            <img src="~/assets/img/order (6).png" />
          </div>
          <div class="card__title">Enjoy your meal and share with friends</div>
          <div class="card__text">
            Satisfied with our service? Why not tell your friends about us?
          </div>
        </div>
      </v-col>
    </v-row>
  </section>
</template>
<script>
export default {
  name: "second",
};
</script>
<style lang="scss" scoped>
.b {
  padding: 60px 20px;
  overflow-x: hidden;
}
.card {
  background-color: rgba(0, 168, 89, 0.08);
  border-radius: 10px;
  width: 320px;
  height: 356px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 0 5px;
  &__title {
    font-weight: bold;
  }
  &__text {
    font-weight: lighter;
    margin: 10px;
  }
}
.text__title {
  font-size: 2rem;
  color: $secondary;
  font-weight: bold;
}
img {
  width: 60%;
}
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .b {
    padding: 60px 10%;
  }
}
@media only screen and (min-width: 992px) {
  .b {
    // width: 80%;
    padding: 60px 10%;
  }
}
</style>