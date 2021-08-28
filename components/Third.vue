<template>
  <section class="c">
    <div class="c__text content section-heading-7">
      <h2 class="secondary--text">Eat at your Convenience</h2>
      <p class="c__body" style="font-size: 1.3rem">
        We are concerned about your convenience in getting your favourite meals
        and dishes from your ‘heartbeat’ restaurants close to you. You get on
        work, class, studies, workout, rest or even laundry, while we get on
        fixing and delivering your preference for breakfast, lunch and dinner.
        Easy to use and convenient for you. your family and friends. Try and see
        how we at CityFood would make you happy.
      </p>
    </div>
    <div class="c__photo">
      <img src="~assets/img/girl.png" alt="" />
    </div>
  </section>
</template>
<script>
export default {
  name: "third",
};
</script>
<style lang="scss" scoped>
.c {
  // margin-top: 10%;
  padding: 60px 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  // background-color: red;
  &__photo {
    // width: 50%;
    margin: 0 0px 33px 0;
  }
  &__body {
    padding: 0 0 0px 0;
  }
  &__title {
    color: $secondary;
    font-weight: bold;
    font-size: 1.4rem;
    padding: 10px 0;
  }
  &__text {
    order: 2;
  }
}
img {
  // width: 80%;
  height: 100%;
  order: 1;
}
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .c {
    // padding: 40px;
    padding: 60px 10%;
    display: flex;
    flex-direction: row;
    &__photo {
      width: 50%;
      margin: 0 20px 0 0;
    }
    &__text {
      width: 40%;
    }
  }
  img {
    height: 90%;
    width: 90%;
    // float: right;
  }
}
@media only screen and (min-width: 992px) {
  .c {
    // padding: 40px;
    padding: 60px 10%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    &__photo {
      width: 50%;
      margin: 0 0 0 0;
    }
    &__text {
      width: 50%;
      // background-color: red;
    }
  }
  img {
    height: 70%;
    width: 70%;
    // float: right;
  }
}
</style>