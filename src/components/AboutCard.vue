<template>
  <div class="about-card">
    <img
      :src="imgSrc"
      :srcset="`${imgSrc} 1x, ${imgSrcRetina} 2x`"
      alt="Card image"
      class="about-card__portrait"
    >
    <div class="about-card__overlay">
      <div class="about-card__socials">
        <a
          href="/"
          class="about-card__social-link"
        >
          <div class="about-card__link-inner">
            <svg
              class="about-card__social-icon"
              xmlns="http://www.w3.org/2000/svg"
              width="1298"
              height="2500"
              viewBox="88.428 12.828 107.543 207.085"
            ><path
              d="M158.232 219.912v-94.461h31.707l4.747-36.813h-36.454V65.134c0-10.658 2.96-17.922 18.245-17.922l19.494-.009V14.278c-3.373-.447-14.944-1.449-28.406-1.449-28.106 0-47.348 17.155-47.348 48.661v27.149H88.428v36.813h31.788v94.461l38.016-.001z"
              fill="#fff"
            /></svg>
          </div>
        </a>
        <a
          href="/"
          class="about-card__social-link"
        >
          <div class="about-card__link-inner">
            <svg
              class="about-card__social-icon"
              xmlns="http://www.w3.org/2000/svg"
              xml:space="preserve"
              viewBox="0 0 248 204"
              width="1298"
              height="2500"
            >
              <path
                fill="#fff"
                d="M221.95 51.29c.15 2.17.15 4.34.15 6.53 0 66.73-50.8 143.69-143.69 143.69v-.04c-27.44.04-54.31-7.82-77.41-22.64 3.99.48 8 .72 12.02.73 22.74.02 44.83-7.61 62.72-21.66-21.61-.41-40.56-14.5-47.18-35.07 7.57 1.46 15.37 1.16 22.8-.87-23.56-4.76-40.51-25.46-40.51-49.5v-.64c7.02 3.91 14.88 6.08 22.92 6.32C11.58 63.31 4.74 33.79 18.14 10.71c25.64 31.55 63.47 50.73 104.08 52.76-4.07-17.54 1.49-35.92 14.61-48.25 20.34-19.12 52.33-18.14 71.45 2.19 11.31-2.23 22.15-6.38 32.07-12.26-3.77 11.69-11.66 21.62-22.2 27.93 10.01-1.18 19.79-3.86 29-7.95-6.78 10.16-15.32 19.01-25.2 26.16z"
              />
            </svg>
          </div>
        </a>
        <a
          href="/"
          class="about-card__social-link"
        >
          <div class="about-card__link-inner">
            <svg
              class="about-card__social-icon"
              version="1.1"
              width="1298"
              height="2500"
              viewBox="0 0 144 144"
            >
              <g>
                <g>
                  <path
                    fill="#fff"
                    d="M71.9,5.4C35.1,5.4,5.3,35.2,5.3,72c0,28.2,17.5,52.3,42.3,62c-0.6-5.3-1.1-13.3,0.2-19.1
			c1.2-5.2,7.8-33.1,7.8-33.1s-2-4-2-9.9c0-9.3,5.4-16.2,12-16.2c5.7,0,8.4,4.3,8.4,9.4c0,5.7-3.6,14.3-5.5,22.2
			c-1.6,6.6,3.3,12,9.9,12c11.8,0,20.9-12.5,20.9-30.5c0-15.9-11.5-27.1-27.8-27.1c-18.9,0-30.1,14.2-30.1,28.9
			c0,5.7,2.2,11.9,5,15.2c0.5,0.7,0.6,1.2,0.5,1.9c-0.5,2.1-1.6,6.6-1.8,7.5c-0.3,1.2-1,1.5-2.2,0.9c-8.3-3.9-13.5-16-13.5-25.8
			c0-21,15.3-40.3,44-40.3c23.1,0,41,16.5,41,38.4c0,22.9-14.5,41.4-34.5,41.4c-6.7,0-13.1-3.5-15.3-7.6c0,0-3.3,12.7-4.1,15.8
			c-1.5,5.8-5.6,13-8.3,17.5c6.2,1.9,12.8,3,19.7,3c36.8,0,66.6-29.8,66.6-66.6C138.5,35.2,108.7,5.4,71.9,5.4z"
                  />
                </g>
              </g>
            </svg>

          </div>
        </a>
        <a
          href="/"
          class="about-card__social-link"
        >
          <div class="about-card__link-inner">
            <svg
              class="about-card__social-icon"
              version="1.1"
              viewBox="0 0 512 512"
              width="1298"
              height="2500"
            ><g id="Edges" /><g id="Symbol"><g><path
              fill="#fff"
              class="st0"
              d="M96.1,23.2c-16.2,6.3-29.9,14.7-43.6,28.4C38.8,65.2,30.4,79,24.1,95.1c-6.1,15.6-10.2,33.5-11.4,59.7    c-1.2,26.2-1.5,34.6-1.5,101.4s0.3,75.2,1.5,101.4c1.2,26.2,5.4,44.1,11.4,59.7c6.3,16.2,14.7,29.9,28.4,43.6    c13.7,13.7,27.4,22.1,43.6,28.4c15.6,6.1,33.5,10.2,59.7,11.4c26.2,1.2,34.6,1.5,101.4,1.5c66.8,0,75.2-0.3,101.4-1.5    c26.2-1.2,44.1-5.4,59.7-11.4c16.2-6.3,29.9-14.7,43.6-28.4c13.7-13.7,22.1-27.4,28.4-43.6c6.1-15.6,10.2-33.5,11.4-59.7    c1.2-26.2,1.5-34.6,1.5-101.4s-0.3-75.2-1.5-101.4c-1.2-26.2-5.4-44.1-11.4-59.7C484,79,475.6,65.2,462,51.6    c-13.7-13.7-27.4-22.1-43.6-28.4c-15.6-6.1-33.5-10.2-59.7-11.4c-26.2-1.2-34.6-1.5-101.4-1.5s-75.2,0.3-101.4,1.5    C129.6,12.9,111.7,17.1,96.1,23.2z M356.6,56c24,1.1,37,5.1,45.7,8.5c11.5,4.5,19.7,9.8,28.3,18.4c8.6,8.6,13.9,16.8,18.4,28.3    c3.4,8.7,7.4,21.7,8.5,45.7c1.2,25.9,1.4,33.7,1.4,99.4s-0.3,73.5-1.4,99.4c-1.1,24-5.1,37-8.5,45.7c-4.5,11.5-9.8,19.7-18.4,28.3    c-8.6,8.6-16.8,13.9-28.3,18.4c-8.7,3.4-21.7,7.4-45.7,8.5c-25.9,1.2-33.7,1.4-99.4,1.4s-73.5-0.3-99.4-1.4    c-24-1.1-37-5.1-45.7-8.5c-11.5-4.5-19.7-9.8-28.3-18.4c-8.6-8.6-13.9-16.8-18.4-28.3c-3.4-8.7-7.4-21.7-8.5-45.7    c-1.2-25.9-1.4-33.7-1.4-99.4s0.3-73.5,1.4-99.4c1.1-24,5.1-37,8.5-45.7c4.5-11.5,9.8-19.7,18.4-28.3c8.6-8.6,16.8-13.9,28.3-18.4    c8.7-3.4,21.7-7.4,45.7-8.5c25.9-1.2,33.7-1.4,99.4-1.4S330.7,54.8,356.6,56z"
            /><path
              fill="#fff"
              class="st1"
              d="M130.9,256.3c0,69.8,56.6,126.3,126.3,126.3s126.3-56.6,126.3-126.3S327,130,257.2,130    S130.9,186.5,130.9,256.3z M339.2,256.3c0,45.3-36.7,82-82,82s-82-36.7-82-82c0-45.3,36.7-82,82-82S339.2,211,339.2,256.3z"
            /><circle
              fill="#fff"
              class="st2"
              cx="388.6"
              cy="125"
              r="29.5"
            /></g></g></svg>
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  imgSrc: {
    type: String,
    required: true,
  },
  imgSrcRetina: {
    type: String,
    required: true,
  },
});
</script>

<style lang="scss" scoped>
.about-card {
  position: relative;
  width: 100%;
  padding-top: 123.6842%;
  background-color: $brand-teal;

  &:focus-within {
    .about-card__portrait {
      transform: translateX(-10px) translateY(-10px);
    }

    .about-card__overlay {
      opacity: 1;
      transform: translateX(-10px) translateY(-10px);
    }
    .about-card__social-link {
      transform: translateY(0);
      opacity: 1;
    }
  }

  &:hover {
    .about-card__portrait {
      transform: translateX(-10px) translateY(-10px);
    }

    .about-card__overlay {
      opacity: 1;
      transform: translateX(-10px) translateY(-10px);
    }
    .about-card__social-link {
      transform: translateY(0);
      opacity: 1;
    }
  }

  &__portrait {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    transition: transform 0.6s;
  }

  &__socials {
    display: flex;
  }

  &__social-link {
    position: relative;
    justify-content: center;
    align-items: center;
    width: 56px;
    height: 56px;
    border-right: 1px solid $brand-pink;
    transform: translateY(30px);
    transition: transform 0.6s, opacity 0.6s;
    opacity: 0;
    z-index: 10;
    
    &:nth-child(2) {
      transition-delay: 0.1s;
    }

    &:nth-child(3) {
      transition-delay: 0.2s;
    }

    &:nth-child(4) {
      transition-delay: 0.3s;
    }

    &:last-child {
      border-right: none;
    }

    & svg path {
        fill: $brand-pink;
    }

    &:hover {
      background-color: $brand-pink;

      & svg path {
        fill: $white;
      }
    }
  }

  &__social-icon {
    max-width: 32px;
    max-height: 32px;
  }

  &__link-inner {
    width: 100%;
    height: 100%;
    background-color: $brand-yellow;
    display: flex;
    justify-content: center;
    align-items: center;
    transition: background-color 0.6s;

    &:hover {
      background-color: $brand-pink;
    }
  }

  &__overlay {
    background-image: linear-gradient(to bottom, #{$brand-pink}E6, #{$brand-yellow}E6);
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 10;
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: transform 0.6s, opacity 0.6s;
  }
}
</style>