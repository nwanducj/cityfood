<template>
  <div>
    <!-- Terms of use-->
    <div class="privacy">
      <div class="wrapper">
        <pdf
          v-for="i in 4"
          :key="i"
          :src="'terms.pdf'"
          :page="i"
          style="height: 100%; width: 100%"
        ></pdf>
      </div>
      <div class="line mx-4"></div>
      <div class="text-center">
        <v-btn class="rounded-lg text-none" color="primary"
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
  name: "ConditionsOfUse",
  components: {
    pdf,
  },
};
</script>

<style lang="scss" scoped>
.wrapper {
  overflow-y: auto;
}
.line {
  border: 2px solid #bab9b9;
  border-radius: 40px;
  margin: 30px 0;
}
.privacy {
  //   width: 80%;
  margin: 10% auto;
  &__texth {
    position: absolute;
    left: 37%;
  }
  &__text {
    margin: 20px 0 0 0;
    text-align: justify;
  }
  &__icon {
    width: 80%;
    height: 80%;
    margin: 0 auto;
    display: inline-block;
  }
}
</style>
