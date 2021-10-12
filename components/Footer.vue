<template>
  <footer>
    <div class="footer mx-auto pa-8">
      <v-row>
        <v-col cols="6" sm="4">
          <div>
            <div class="title">Resources</div>
            <div @click="$router.push('/privacy-policy')">Privacy policy</div>
            <div @click="$router.push('/terms-of-service')">
              Terms of service
            </div>
          </div>
        </v-col>
        <v-col cols="6" sm="4">
          <div>
            <div class="title">Discover</div>
            <div>
              <v-btn
                text
                x-small
                class="text-none white--text pa-0"
                @click="$emit('gotoFourth')"
                >For Vendors</v-btn
              >
            </div>
            <div>
              <v-btn
                text
                x-small
                class="text-none white--text pa-0"
                @click="$emit('gotoSixth')"
                >Partnerships</v-btn
              >
            </div>
          </div>
        </v-col>
        <v-col cols="6" sm="4">
          <div>
            <div class="title">Follow us</div>
            <div class="d-flex align-items">
              <v-icon color="white" size="18" class="mr-2">mdi-facebook</v-icon
              ><a href="https://www.facebook.com/cityfood_ng" target="blank"
                >Facebook</a
              >
            </div>
            <div>
              <v-icon color="white" size="18" class="mr-2">mdi-twitter</v-icon
              ><a href="https://www.twitter.com/cityfood_ng" target="blank"
                >Twitter</a
              >
            </div>
            <div>
              <v-icon color="white" size="18" class="mr-2">mdi-linkedin</v-icon
              ><a
                href="https://www.linkedin.com/company/cityfood-ng"
                target="blank"
                >LinkedIn</a
              >
            </div>
            <div>
              <v-icon color="white" size="18" class="mr-2">mdi-instagram</v-icon
              ><a href="https://www.instagram.com/cityfood_ng" target="blank"
                >Instagram</a
              >
            </div>
          </div>
        </v-col>
      </v-row>
    </div>
    <div class="text-center py-8">
      CityFood, <br />
      Enugu City, Enugu 400210, Nigeria <br />
      Copyright@2021
    </div>
  </footer>
</template>
<script>
export default {
  name: "Footer",
};
</script>
<style lang="scss" scoped>
a {
  color: white;
}
footer {
  background-color: lighten(black, 53%);
  color: white;
  .title {
    font-weight: 600;
    color: white;
  }
}
@media only screen and (min-width: 992px) {
  .footer {
    width: 80%;
  }
}
</style>