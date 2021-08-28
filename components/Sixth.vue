<template>
  <section class="full f d-flex align-center justify-center" ref="myRef">
    <div class="holder">
      <div class="connect">Connect With Us</div>
      <div class="pr-8">
        If you require further assistance or would like to reach us for general
        inquiries, please call us on
        <span class="secondary--text">+2348140150211</span> or email
        <span class="secondary--text">info@cityfood.com</span>
      </div>
      <div class="d-flex my-4">
        <v-avatar circle size="40" color="primary" class="mr-2"
          ><v-icon color="white" size="18">mdi-facebook</v-icon></v-avatar
        >
        <v-avatar circle size="40" color="primary" class="mx-2"
          ><v-icon color="white" size="18">mdi-twitter</v-icon></v-avatar
        >
        <v-avatar circle size="40" color="primary" class="mx-2"
          ><v-icon color="white" size="18">mdi-linkedin</v-icon></v-avatar
        >
        <v-avatar circle size="40" color="primary" class="mx-2"
          ><v-icon color="white" size="18">mdi-instagram</v-icon></v-avatar
        >
        <v-avatar circle size="40" color="primary" class="mx-2"
          ><v-icon color="white" size="18">mdi-whatsapp</v-icon></v-avatar
        >
      </div>
      <div class="mt-16 mb-4 newsletter">Subscribe to our Newsletter</div>
      <div class="d-block d-sm-block d-md-flex">
        <v-text-field outlined placeholder="Email Address" dense></v-text-field>
        <v-btn
          color="primary"
          class="text-none float-end elevation-0 text-caption ml-2"
          style="height: 40px"
          >Subscribe Newsletter</v-btn
        >
      </div>
    </div>
    <img src="~assets/img/amico.png" alt="" class="d-none d-sm-block" />
  </section>
</template>
<script>
export default {
  name: "sixth",
  props: ["myRef"],
};
</script>
<style lang="scss" scoped>
.connect {
  font-weight: bold;
  font-size: 1.4rem;
}
.f {
  padding: 60px 8%;
  background-color: #1eb36d14;
}
.newsletter {
  font-size: 1.4rem;
  font-weight: bold;
}
img {
  width: 364px;
  height: 313px;
  margin: 0 0 0 30%;
  margin: 0 auto;
}
.v-btn {
  height: 150px;
}
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .f {
    padding: 60px 10%;
    margin: 0% auto;
  }
  .holder {
    width: 50%;
  }
}
@media only screen and (min-width: 992px) {
  .f {
    padding: 60px 10%;
    margin: 0% auto;
  }
  .holder {
    width: 50%;
  }
}
</style>