<template>
  <div>
    <div class="header">
      <div class="d-flex align-center ml-sm-16 py-4">
        <img class="icon" src="~assets/img/cityfoodpng 1.png" />
        <img class="cityfood" src="~assets/img/cityfoodpng 2.png" />
      </div>
      <div class="head__privacy d-flex pa-2 align-center">
        <div @click="$router.go(-1)" class="mt-2 ml-2 ml-sm-16">
          <svg
            width="23"
            height="20"
            viewBox="0 0 73 67"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g filter="url(#filter0_d)">
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M30.75 3.25003C30.7506 2.70258 30.5636 2.16868 30.2154 1.72304C29.8671 1.2774 29.375 0.942319 28.8079 0.764694C28.2407 0.58707 27.6269 0.575789 27.0524 0.732429C26.4779 0.88907 25.9714 1.20579 25.6038 1.63828L5.47879 25.2633C5.0862 25.7241 4.87305 26.2912 4.87305 26.875C4.87305 27.4588 5.0862 28.026 5.47879 28.4868L25.6038 52.1118C25.9714 52.5443 26.4779 52.861 27.0524 53.0176C27.6269 53.1743 28.2407 53.163 28.8079 52.9854C29.375 52.8077 29.8671 52.4727 30.2154 52.027C30.5636 51.5814 30.7506 51.0475 30.75 50.5V40.0263C46.2147 40.3203 53.6437 43.0004 57.3754 45.9142C60.9232 48.6835 61.5729 51.9412 62.2485 55.3537L62.4239 56.233C62.5529 56.8623 62.9293 57.4268 63.4823 57.8203C64.0353 58.2139 64.7267 58.4094 65.4265 58.37C66.1264 58.3307 66.7863 58.0592 67.2822 57.6067C67.7781 57.1541 68.0758 56.5517 68.1193 55.9128C68.6109 48.6993 67.872 38.2465 62.2917 29.5027C56.8752 21.016 47.1203 14.4903 30.75 13.8078V3.25003Z"
                fill="#45484A"
                fill-opacity="0.8"
                shape-rendering="crispEdges"
              />
            </g>
            <defs>
              <filter
                id="filter0_d"
                x="0.873047"
                y="0.622681"
                width="71.3729"
                height="65.7523"
                filterUnits="userSpaceOnUse"
                color-interpolation-filters="sRGB"
              >
                <feFlood flood-opacity="0" result="BackgroundImageFix" />
                <feColorMatrix
                  in="SourceAlpha"
                  type="matrix"
                  values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                  result="hardAlpha"
                />
                <feOffset dy="4" />
                <feGaussianBlur stdDeviation="2" />
                <feComposite in2="hardAlpha" operator="out" />
                <feColorMatrix
                  type="matrix"
                  values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"
                />
                <feBlend
                  mode="normal"
                  in2="BackgroundImageFix"
                  result="effect1_dropShadow"
                />
                <feBlend
                  mode="normal"
                  in="SourceGraphic"
                  in2="effect1_dropShadow"
                  result="shape"
                />
              </filter>
            </defs>
          </svg>
        </div>
        <div
          class="secondary--text font-weight-bold mx-auto mt-1 privacy__texth"
        >
          Privacy Policy
        </div>
      </div>
    </div>
    <div class="privacy">
      <div class="d-flex">
        <img class="privacy__icon" src="~assets/img/Privacy icon.png" />
      </div>
      <div class="line"></div>
      <div class="wrapper">
        <pdff
          v-for="i in 10"
          :key="i"
          :page="i"
          :src="'policy.pdf'"
          style="height: 100%"
        ></pdff>
      </div>
      <div class="line"></div>
      <div class="text-center">
        <v-btn class="rounded-lg text-none" color="primary"
          >Download Privacy Policy</v-btn
        >
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import pdff from "vue-pdf";
export default {
  name: "index",
  components: {
    pdff,
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
.header {
  z-index: 2;
  position: fixed;
  top: 0;
  width: 100%;
  background-color: white;
}
.head__privacy {
  background-color: lighten($primary, 25%);
  display: block;
  // width: 80%;
  padding: 0 20%;
}
.icon {
  height: 41px;
  width: 70px;
}
.cityfood {
  height: 22px;
  width: 70px;
}
.privacy {
  width: 80%;
  margin: 150px auto;
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
@media only screen and (min-width: 768px) and (max-width: 992px) {
  .privacy {
    width: 70%;
    margin: 150px auto;
    &__texth {
      position: absolute;
      left: 43%;
    }
    &__text {
      margin: 70px 0 0 0;
      text-align: justify;
    }
    &__icon {
      width: 20%;
      height: 20%;
      margin: 0 auto;
      display: inline-block;
    }
  }
}
@media only screen and (min-width: 992px) {
  .privacy {
    width: 70%;
    margin: 150px auto;
    &__texth {
      position: absolute;
      left: 46%;
    }
    &__text {
      margin: 70px 0 0 0;
      text-align: justify;
    }
    &__icon {
      width: 20%;
      height: 20%;
      margin: 0 auto;
      display: inline-block;
    }
  }
}
</style>
