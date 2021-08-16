<template>
  <section class="full c">
    <div class="c__text">
      <div class="c__title">Eat at your Convenience</div>
      <div class="c__body">
        We are concerned abiut your convenience in getting your favourite meals and dishes from your ‘heartbeat’ restaurants close to you.
        You get on work, class, studies, workout, rest or even laundry, while we get on fixing and delivering your preference for breakfast, lunch and dinner.
        Easy to use and convenient for you. your family and friends. Try and see how we at CityFood would make you happy.
      </div>
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
  padding: 20px;
  align-items: center;
  &__body {
    padding: 0 0 20px 0;
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
  width: 100%;
  order: 1;
}
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .c {
    padding: 60px;
    display: flex;
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
    float: right;
  }
}
@media only screen and (min-width: 992px) {
  .c {
    padding: 60px;
    display: flex;
    &__photo {
      width: 50%;
      margin: 0 20px 0 0;
    }
    &__text {
      width: 30%;
    }
  }
  img {
    height: 70%;
    width: 70%;
    float: right;
  }
}
</style>