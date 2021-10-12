<template>
  <div style="background-color: #f8765a1f" class="f">
    <div class="hero-area-l-13 position-relative overflow-hidden">
      <div class="container">
        <div class="row position-relative justify-content-center">
          <div
            class="offset-xl-1 col-xl-5 col-lg-6 col-md-8 col-sm-9"
            data-aos="fade-left"
            data-aos-duration="800"
            data-aos-once="true"
          >
            <div class="content">
              <h1>
                Get your food
                <span class="primary--text font-weight-bold">on the Go!</span>
              </h1>

              <p>
                Our job is to satisfy you with delicious meals from your
                favourite restaurants nearby, without moving an inch from your
                sofa, office, school or even bus station.
                <span class="secondary--text font-weight-bold">Order Now!</span>
              </p>
              <div class="apps-btn">
                <a href="#" class="app-store"
                  ><img src="~assets/img/google.png" alt=""
                /></a>
                <a href="#" class="app-store"
                  ><img src="~assets/img/apple.png" alt=""
                /></a>
              </div>
            </div>
          </div>
          <div
            class="col-xl-6 col-lg-6 col-sm-9"
            data-aos="fade-right"
            data-aos-duration="800"
            data-aos-once="true"
          >
            <div class="photo">
              <img src="~assets/img/fone.png" alt="" class="w-100" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "first",
};
</script>
<style lang="scss" scoped>
.city {
  font-size: 3rem;
  color: $primary;
}
.photo {
  top: 2%;
}
.f {
  padding: 20px 20px;
}

@media only screen and (min-width: 768px) and (max-width: 992px) {
  .photo {
    top: 2%;
  }
  .f {
    padding: 60px 10%;
    margin: 0% auto;
  }
}

@media only screen and (min-width: 992px) {
  .photo {
    position: absolute;
    top: 3%;
  }
  .f {
    padding: 60px 10%;
    margin: 0% auto;
  }
}
</style>