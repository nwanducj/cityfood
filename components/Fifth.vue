<template>
  <div class="e">
    <div class="content-area-l-13-2 position-relative overflow-hidden">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-md-12">
            <div class="border-bottom">
              <div class="row justify-content-center">
                <div class="col-xl-11">
                  <div
                    class="
                      row
                      align-items-center
                      justify-content-center justify-content-lg-start
                    "
                  >
                    <div
                      class="col-lg-6 col-md-6 col-sm-6 big-phone"
                      data-aos="fade-right"
                      data-aos-duration="800"
                      data-aos-once="true"
                    >
                      <div class="app-image-position-l-13">
                        <img src="~assets/img/fone.png" alt="" class="w-100" />
                      </div>
                    </div>
                    <div
                      class="
                        offset-lg-1
                        col-lg-5 col-md-8 col-sm-10
                        position-relative
                      "
                      data-aos="fade-left"
                      data-aos-duration="800"
                      data-aos-once="true"
                    >
                      <div class="content section-heading-7">
                        <h2>
                          Download Our App today and start experiencing prompt
                          food delivery service
                        </h2>
                        <div class="d-flex text-caption">
                          <img src="~assets/img/qr.png" alt="" class="qr" />
                          <div class="ml-4">
                            <p>
                              <span
                                >Use your Phone camera to scan and download City
                                Food App </span
                              ><br />
                            </p>
                            <p class="mt-4">
                              <span
                                >Available on
                                <span class="secondary--text font-weight-bold"
                                  >iOS</span
                                >
                                and
                                <span class="secondary--text font-weight-bold"
                                  >Android</span
                                ></span
                              >
                            </p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "fifth",
};
</script>
<style lang="scss" scoped>
.e {
  padding: 60px 20px;
}
.download {
  font-size: 1.6rem;
  font-weight: bold;
}
.photo {
  // display: none;
  width: 100%;
  margin: 0 auto;
  &__holder {
    width: 90%;
  }
}
.text {
  margin: 0% 0 0 0;
  width: 100%;
}
.qr {
  width: 100%;
  height: 100%;
}
.big-phone {
  display: none;
}
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .e {
    flex-direction: row;
    padding: 60px 10% 0 10%;
    margin: 0% auto;
  }
  .qr {
    width: 30%;
  }
  .big-phone {
    display: none;
  }
  .photo {
    display: block;
    width: 80%;
    order: 1;
    z-index: 2;
    left: 12%;
    margin: -5% 0 25% 0;
    float: right;
    &__holder {
      width: 45%;
    }
  }
  .text {
    margin: 25% 10% 0 10%;
    // width: 100%;
    z-index: 3;
    order: 2;
    padding: 0% 0 0 0%;
    width: 100%;
    display: flex;
    flex-direction: column;
  }
}
@media only screen and (min-width: 992px) {
  .download {
    font-size: 2rem;
  }
  .big-phone {
    display: block;
  }
  .qr {
    width: 30%;
  }
  .e {
    flex-direction: row;
    padding: 60px 10% 0 10%;
    margin: 0% auto;
    // width: 80%;
  }
  .photo {
    display: block;
    width: 40%;
    z-index: 2;
    position: absolute;
    left: 12%;
    margin: -5% 0 0 0;
    &__holder {
      width: 45%;
    }
  }
  .text {
    z-index: 3;
    order: 2;
    padding: 0% 0 0 30%;
    width: 70%;
    display: flex;
    flex-direction: column;
  }
}
</style>