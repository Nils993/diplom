<template>
  <header class="header center">
    <div class="logo">
      <a href="/">
        <svg
          width="55"
          height="59"
          viewBox="0 0 55 59"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <g filter="url(#filter0_d_102_283)">
            <path
              d="M34.7014 27.022L30.6949 17.8445L29.8213 17.2388L28.797 16.9127L27.4113 16.54L25.7846 17.2388L24.7001 17.8445L28.797 27.022H34.7014Z"
              fill="url(#paint0_linear_102_283)"
            />
          </g>
          <g filter="url(#filter1_d_102_283)">
            <path
              d="M20.3231 23.9535L24.3296 33.1525L25.2032 33.7595L26.2274 34.0864L27.6131 34.46L29.2399 33.7595L30.3243 33.1525L26.2274 23.9535H20.3231Z"
              fill="url(#paint1_linear_102_283)"
            />
          </g>
          <path
            d="M24.4859 17.9646L18.2659 26.9553L24.4859 27.022L28.9822 17.9646C29.2979 17.038 30.2856 17.5785 30.74 17.9646C28.798 14.4065 25.7614 16.4821 24.4859 17.9646Z"
            fill="white"
          />
          <path
            d="M30.5141 33.0354L36.7341 24.0447L30.5141 23.978L26.0178 33.0354C25.7021 33.962 24.7144 33.4215 24.26 33.0354C26.202 36.5935 29.2386 34.5179 30.5141 33.0354Z"
            fill="white"
          />
          <defs>
            <filter
              id="filter0_d_102_283"
              x="4.70013"
              y="0.540039"
              width="50.0013"
              height="50.4819"
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
              <feGaussianBlur stdDeviation="10" />
              <feComposite in2="hardAlpha" operator="out" />
              <feColorMatrix
                type="matrix"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"
              />
              <feBlend
                mode="normal"
                in2="BackgroundImageFix"
                result="effect1_dropShadow_102_283"
              />
              <feBlend
                mode="normal"
                in="SourceGraphic"
                in2="effect1_dropShadow_102_283"
                result="shape"
              />
            </filter>
            <filter
              id="filter1_d_102_283"
              x="0.323059"
              y="7.95349"
              width="50.0013"
              height="50.5065"
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
              <feGaussianBlur stdDeviation="10" />
              <feComposite in2="hardAlpha" operator="out" />
              <feColorMatrix
                type="matrix"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"
              />
              <feBlend
                mode="normal"
                in2="BackgroundImageFix"
                result="effect1_dropShadow_102_283"
              />
              <feBlend
                mode="normal"
                in="SourceGraphic"
                in2="effect1_dropShadow_102_283"
                result="shape"
              />
            </filter>
            <linearGradient
              id="paint0_linear_102_283"
              x1="33.6653"
              y1="27.022"
              x2="28.9137"
              y2="18.1327"
              gradientUnits="userSpaceOnUse"
            >
              <stop />
              <stop offset="0.494792" stop-color="white" />
              <stop offset="1" stop-color="white" />
            </linearGradient>
            <linearGradient
              id="paint1_linear_102_283"
              x1="21.3592"
              y1="23.9535"
              x2="26.1281"
              y2="32.8543"
              gradientUnits="userSpaceOnUse"
            >
              <stop stop-color="#0C0C0C" />
              <stop offset="0.494792" stop-color="white" />
              <stop offset="1" stop-color="white" />
            </linearGradient>
          </defs>
        </svg>
      </a>
      <span class="logo-text">thewatchspot</span>
    </div>
    <NavComp />
    <div class="header-number">
      <p>+380 (68) 443-94-26</p>
    </div>
  </header>
</template>

<script>
import NavComp from "@/components/NavComp.vue";

export default {
  components: {
    NavComp,
  },
};
</script>

<style lang="scss" scoped>
.header {
  background-color: rgb(20, 20, 20);
  padding-top: 27px;
  padding-bottom: 80px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  justify-content: space-between;
  &-number {
    color: var(--white);
    font-size: 9px;
    font-weight: 400;
    line-height: 12px;
    text-align: center;
    text-transform: uppercase;
    border: solid 1px var(--darkGreen);
    border-radius: 8px;
    background: var(--darkGreen);
    padding: 18px 36px;
  }
}
.logo {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  &-text {
    color: var(--white);
    font-size: 15px;
    font-weight: 400;
    line-height: 15px;
    text-align: center;
  }
}
@media (max-width: 700px) {
  .header-number {
    display: none;
  }
}
@media (max-width: 500px) {
  .logo {
    z-index: 10;
  }
}
</style>
