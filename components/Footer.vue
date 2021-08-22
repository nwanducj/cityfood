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
            <div>For Vendors</div>
            <div>Partnerships</div>
          </div>
        </v-col>
        <v-col cols="6" sm="4">
          <div>
            <div class="title">Follow us</div>
            <div class="d-flex align-items">
              <v-icon color="white" size="18" class="mr-2">mdi-facebook</v-icon
              >Facebook
            </div>
            <div>
              <v-icon color="white" size="18" class="mr-2">mdi-twitter</v-icon
              >Twitter
            </div>
            <div>
              <v-icon color="white" size="18" class="mr-2">mdi-linkedin</v-icon
              >LinkedIn
            </div>
            <div>
              <v-icon color="white" size="18" class="mr-2">mdi-instagram</v-icon
              >Instagram
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