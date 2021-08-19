<template>
  <section class="full a">
    <div class="main">
      <div class="main__title font-weight-bold">
        The Food is for the <span class="city">City</span>
      </div>
      <div class="main__text">
        Our job is to satisfy you with delicious meals from your favourite
        restaurants nearby, without moving an inch from your sofa, office,
        school or even bus station. <span class="order">Order Now!</span>
      </div>
      <div class="buttons">
        <div class="button d-flex align-center elevation-1">
          <div>
            <svg
              width="19"
              height="22"
              viewBox="0 0 32 37"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g clip-path="url(#clip0)">
                <path
                  d="M18.3897 17.3495L23.0896 12.6492C14.5051 7.56524 1.82027 0.106667 1.1034 0L1.04602 0.00588506L18.3897 17.3495Z"
                  fill="#05D86B"
                />
                <path
                  d="M0.00588506 1.04644L0 1.10345V35.6782L0.00551724 35.733L17.3491 18.3897L0.00588506 1.04644Z"
                  fill="#09D5AC"
                />
                <path
                  d="M18.392 19.4325L1.04907 36.7757L1.10351 36.782C1.82369 36.6672 14.5064 29.2123 23.0897 24.1306L18.392 19.4325Z"
                  fill="#F93D29"
                />
                <path
                  d="M30.8966 17.2874C30.8966 17.2874 28.185 15.6697 24.3991 13.4253L19.4325 18.3923L24.3969 23.3567C28.1839 21.1119 30.8966 19.4943 30.8966 19.4943C31.4877 19.1838 32 19.0003 32 18.3908C32 17.7817 31.4174 17.5724 30.8966 17.2874Z"
                  fill="#FF980A"
                />
              </g>
              <defs>
                <clipPath id="clip0">
                  <rect width="32" height="36.782" fill="white" />
                </clipPath>
              </defs>
            </svg>
          </div>
          <div class="ml-4" style="font-size: 0.8rem">
            Get IN ON<br />
            <span class="font-weight-bold">Google Play</span>
          </div>
        </div>
        <div class="button d-flex align-center elevation-1">
          <div>
            <svg
              width="28"
              height="28"
              viewBox="0 0 48 48"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M18.188 42.012C16.9304 41.9439 15.747 41.3955 14.882 40.48C13.8472 39.4845 12.9238 38.3793 12.128 37.184C10.885 35.404 9.90238 33.4557 9.21 31.398C8.42641 29.1843 8.01419 26.8562 7.99 24.508C7.92913 22.2039 8.49972 19.9271 9.64 17.924C10.4752 16.4802 11.6664 15.2745 13.1 14.422C14.5178 13.5731 16.1356 13.1162 17.788 13.098C19.0336 13.1717 20.2577 13.4564 21.408 13.94C22.326 14.344 23.29 14.628 24.28 14.784C25.372 14.5552 26.4391 14.2203 27.466 13.784C28.6813 13.3095 29.9681 13.0437 31.272 12.998C31.446 12.998 31.618 12.998 31.784 13.018C34.644 13.1 37.304 14.504 38.984 16.818C37.6729 17.5193 36.5819 18.5704 35.8323 19.8545C35.0827 21.1386 34.7039 22.6055 34.738 24.092C34.7249 25.2287 34.9529 26.3552 35.4069 27.3973C35.8609 28.4395 36.5307 29.3736 37.372 30.138C38.138 30.868 39.03 31.452 40.004 31.864C39.804 32.464 39.574 33.044 39.33 33.628C38.776 34.9185 38.0925 36.1495 37.29 37.302C36.5312 38.4565 35.6479 39.5243 34.656 40.486C33.7513 41.3838 32.5452 41.9134 31.272 41.972C30.1927 41.9242 29.1325 41.671 28.148 41.226C27.0864 40.7635 25.9456 40.5103 24.788 40.48C23.5978 40.5035 22.4232 40.7554 21.328 41.222C20.3821 41.6488 19.3715 41.9144 18.338 42.008L18.188 42.012ZM24.488 12.998C24.338 12.998 24.188 12.998 24.038 12.98C24.0065 12.7419 23.9898 12.5021 23.988 12.262C24.0534 10.2643 24.8341 8.35647 26.188 6.886C26.9452 6.04091 27.8631 5.35493 28.888 4.868C29.8431 4.37631 30.8869 4.08051 31.958 3.998C31.988 4.26 31.988 4.516 31.988 4.76C31.9599 6.72633 31.2211 8.61605 29.908 10.08C29.2723 10.9324 28.4576 11.6354 27.5213 12.1395C26.585 12.6436 25.5496 12.9366 24.488 12.998Z"
                fill="white"
              />
            </svg>
          </div>
          <div class="ml-4">
            Download on the<br />
            <span class="font-weight-bold">Apple Store</span>
          </div>
        </div>
      </div>
    </div>
    <div class="image d-flex justify-center">
      <img src="~assets/img/fone.png" alt="" class="mx-auto" />
    </div>
  </section>
</template>
<script>
export default {
  name: "first",
};
</script>
<style lang="scss" scoped>
img {
  width: 653px;
  height: 670px;
  display: none;
  margin: 30% 0 0 0;
}
.a {
  background-color: #f8765a1f;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 30px 30px;
}
.main {
  width: 100%;
  font-family: "Josefin Sans", sans-serif;
  margin: 10% 0 0 0;
  &__title {
    font-size: 3rem;
    line-height: 3.2rem;
  }
  .city {
    font-size: 3rem;
    color: $primary;
  }
  &__text {
    font-size: 1.5rem;
    padding: 15px 0;
  }
  .order {
    font-size: bold;
    color: #00a859;
    font-weight: bold;
  }
}
.button {
  background-color: $accent;
  color: white;
  padding: 5px 20px;
  border-radius: 10px;
  width: 70%;
  height: 48px;
  line-height: 1.2rem;
  margin: 10px 0;
  justify-content: center;
}

@media only screen and (min-width: 768px) and (max-width: 992px) {
  .main {
    width: 70%;
  }
  .buttons {
    display: flex;
  }
  .button {
    width: 195px;
    margin: 0 10px 0 0;
  }
  img {
    display: none;
    width: 50%;
  }
}
@media only screen and (min-width: 992px) {
  .main {
    width: 40%;
    padding: 0 40px;
  }
  .buttons {
    display: flex;
  }
  .button {
    width: 210px;
    margin: 0 10px 0 0;
  }
  img {
    display: block;
    width: 80%;
    height: 80%;
  }
}
</style>