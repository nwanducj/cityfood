<template>
  <section class="full e d-sm-flex align-center">
    <div class="text">
      <div class="download my-2 mb-8">
        Download Our App today and start experiencing prompt food delivery
        service
      </div>
      <div class="d-flex text-caption align-center">
        <div><img src="~assets/img/qr.png" alt="" class="qr" /></div>
        <div class="ml-4">
          Use your Phone camera to scan and download City Food App <br />
          <span>Available on <span>ios</span> and <span>Android</span></span>
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
  padding: 20px;
}
.download {
  font-size: 1.4rem;
  font-weight: bold;
}
.photo {
  width: 80%;
  order: 1;
  margin: auto auto;
  display: block;
}
.text {
  order: 2;
  margin: 10% 0 0 0;
  width: 80%;
}
.qr {
  width: 100px;
  height: 100px;
}
@media only screen and (min-width: 600px) and (max-width: 960px) {
  .photo {
    display: block;
    width: 100%;
    order: 2;
  }
  .text {
    background-color: white;
    order: 1;
    margin: 0 0 0 0;
    width: 100%;
  }
}
@media only screen and (min-width: 960px) {
  .e {
    //   padding: 20px;
    margin: 60px;
  }
  .photo {
    display: block;
  }
  .text {
    order: 2;
    margin: 0% 100px 0 0;
    width: 50%;
    display: flex;
    flex-direction: column;
    // justify-content: flex-start;
    align-items: flex-start;
  }
}
</style>