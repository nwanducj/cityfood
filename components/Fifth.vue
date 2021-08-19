<template>
  <section class="full e">
    <div class="d-md-flex justify-end">
      <div class="text">
        <div class="download my-2 mb-8">
          Download Our App today and start experiencing prompt food delivery
          service
        </div>
        <div class="d-flex text-caption align-center">
          <div><img src="~assets/img/qr.png" alt="" class="qr" /></div>
          <div class="ml-4">
            <div>
              Use your Phone camera to scan and download City Food App <br />
            </div>
            <div class="mt-4">
              <span
                >Available on
                <span class="secondary--text font-weight-bold">iOS</span> and
                <span class="secondary--text font-weight-bold"
                  >Android</span
                ></span
              >
            </div>
          </div>
        </div>
      </div>
      <img src="~assets/img/phone-below.png" alt="" class="photo" />
    </div>
  </section>
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