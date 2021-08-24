<template>
  <div>
    <div class="header">
      <div class="d-flex align-center ml-sm-16 py-4">
        <img class="icon" src="~assets/img/cityfoodpng 1.png" />
        <img class="cityfood" src="~assets/img/cityfoodpng 2.png" />
      </div>
    </div>
    <div class="wrapper">
      <pdf
        v-for="i in 10"
        :key="i"
        :page="i"
        :src="'terms.pdf'"
        style="height: 100%"
      ></pdf>
      <div class="line mx-4"></div>
      <div class="text-center my-8">
        <v-btn class="rounded-lg text-none my-2" color="primary"
          >Download Terms of Service</v-btn
        >
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import pdf from "vue-pdf";
export default {
  name: "index",
  components: {
    pdf,
  },
};
</script>
<style lang="scss" scoped>
.header {
  z-index: 2;
  position: fixed;
  top: 0;
  width: 100%;
  background-color: white;
}
.icon {
  height: 41px;
  width: 70px;
}
.cityfood {
  height: 22px;
  width: 70px;
}
.wrapper {
  overflow-y: auto;
  overflow-x: hidden;
  margin-top: 12%;
}
.line {
  border: 2px solid #bab9b9;
  border-radius: 40px;
  margin: 30px 0 0 0;
}

@media only screen and (min-width: 768px) and (max-width: 992px) {
  .wrapper {
    overflow-y: auto;
    overflow-x: hidden;
    margin-top: 3%;
  }
}
@media only screen and (min-width: 992px) {
  .wrapper {
    overflow-y: auto;
    overflow-x: hidden;
    margin-top: 0%;
  }
}
</style>
