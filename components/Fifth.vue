<template>
  <div>
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
                      class="col-lg-6 col-md-8 col-sm-10"
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
                          <div class="photo__holder">
                            <img
                              src="~assets/img/qr.png"
                              alt=""
                              class="qr"
                              style="display: inline-block"
                            />
                          </div>
                          <div class="ml-4">
                            <p>
                              Use your Phone camera to scan and download City
                              Food App <br />
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
  margin-top: 30%;
  padding: 20px 20px 0 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
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
    width: 70%;
  }
}
.text {
  margin: 0% 0 0 0;
  width: 100%;
}
.qr {
  width: 120px;
  height: 120px;
}
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .e {
    flex-direction: column;
    margin: 0px;
    width: 80%;
    justify-content: center;
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
  .e {
    flex-direction: row;
    margin: 0px;
    width: 80%;
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