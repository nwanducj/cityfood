<template>
  <section class="full c">
    <div class="c__text">
      <div class="c__title">Eat at your Convenience</div>
      <div class="c__body">
        Are you searching for Qr Code png images or vector? Choose from 2400+ Qr
        Code graphic resources and download in the form of PNG, EPS, AI or PSD.
        Choose from 2400+ Qr Code graphic resources and download in the form of
        PNG, EPS, AI or PSD. Qr Code graphic resources and download in the form
        of PNG, EPS, AI or PSD. Qr Code graphic resources and download in the
        form of PNG, EPS, AI or PSD. Qr Code graphic resources and download in
        the form of PNG, EPS, AI or PSD.
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