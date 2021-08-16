<template>
  <section class="full e">
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
            <span>Available on <span class="secondary--text font-weight-bold">iOS</span> and <span class="secondary--text font-weight-bold">Android</span></span>
          </div>
          </div>
      </div>
    </div>
    <img src="~assets/img/phone-below.png" alt="" class="photo" />
  </section>
</template>
<script>
export default {
  name: "fifth",
};
</script>
<style lang="scss" scoped>
.e {
  // background-color: red;
  padding: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.download {
  font-size: 1.4rem;
  font-weight: bold;
}
.photo {
  width: 350px;
  // order: 1;
  margin: auto auto;
  // display: none;
}
.text {
  // order: 2;
  margin: 0% 0 0 0;
  width: 100%;
}
.qr {
  width: 100px;
  height: 100px;
}
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .e {
    flex-direction: row;
  }
  .photo {
    display: block;
    width: 80%;
    order: 1;
  }
  .text {
    background-color: white;
    order: 2;
    margin: 0 0 0 0;
    width: 100%;
  }
}
@media only screen and (min-width: 992px) {
  .e {
    //   padding: 20px;
    flex-direction: row;
    margin: 60px;
  }
  .photo {
    display: block;
    width: 100%;
    order: 1;
  }
  .text {
    order: 2;
    margin: 0% 100px 0 0;
    width: 50%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>