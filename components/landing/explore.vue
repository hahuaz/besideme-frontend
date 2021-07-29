<template>
  <div class="explore grid grid-cols-4">
    <div
      class="explore__title col-span-1 relative p-12 text-center text-gray-100"
    >
      <p class="font-semibold text-4xl">Explore The Best Cities</p>
      <p class="mt-8">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores soluta
        architecto iure labore id, sint amet ab dolore quod accusamus.
      </p>
      <div class="background--image" style=""></div>
    </div>
    <div class="col-span-3">
      <splide
        :options="{
          rewind: true,
          perPage: 3,
          arrows: false,
          pagination: true,
          pauseOnHover: true,
        }"
      >
        <splide-slide>
          <div class="paris city relative h-[550px] p-12">
            <div class="absolute bottom-8 left-8 text-white space-y-4">
              <a href="#">
                <span
                  class="
                    proporty__button
                    opacity-0
                    py-2
                    px-4
                    rounded-md
                    bg-c-blue
                    text-sm
                  "
                  >5 Proporties ></span
                >
              </a>
              <p class="font-semibold text-2xl">Paris</p>
              <p class="text-sm w-4/5">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illo
                aliquam repellat molestias deserunt, neque vel.
              </p>
            </div>
            <div
              class="background--image"
              :style="{ backgroundImage: `url(${paris})` }"
            ></div>
          </div>
        </splide-slide>
        <splide-slide>
          <div class="amsterdam city relative h-[550px] p-12">
            <div class="absolute bottom-8 left-8 text-white space-y-4">
              <a href="#">
                <span
                  class="
                    proporty__button
                    opacity-0
                    py-2
                    px-4
                    rounded-md
                    bg-c-blue
                    text-sm
                  "
                  >7 Proporties ></span
                >
              </a>
              <p class="font-semibold text-2xl">Amsterdam</p>
              <p class="text-sm w-4/5">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illo
                aliquam repellat molestias deserunt, neque vel.
              </p>
            </div>
            <div
              class="background--image"
              :style="{ backgroundImage: `url(${amsterdam})` }"
            ></div>
          </div> </splide-slide
        ><splide-slide>
          <div class="newyork city relative h-[550px] p-12">
            <div class="absolute bottom-8 left-8 text-white space-y-4">
              <a href="#">
                <span
                  class="
                    proporty__button
                    opacity-0
                    py-2
                    px-4
                    rounded-md
                    bg-c-blue
                    text-sm
                  "
                  >4 Proporties ></span
                >
              </a>
              <p class="font-semibold text-2xl">Newyork</p>
              <p class="text-sm w-4/5">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illo
                aliquam repellat molestias deserunt, neque vel.
              </p>
            </div>
            <div
              class="background--image"
              :style="{ backgroundImage: `url(${newyork})` }"
            ></div>
          </div> </splide-slide
        ><splide-slide>
          <div class="berlin city relative h-[550px] p-12">
            <div class="absolute bottom-8 left-8 text-white space-y-4">
              <a href="#">
                <span
                  class="
                    proporty__button
                    opacity-0
                    py-2
                    px-4
                    rounded-md
                    bg-c-blue
                    text-sm
                  "
                  >2 Proporties ></span
                >
              </a>
              <p class="font-semibold text-2xl">Berlin</p>
              <p class="text-sm w-4/5">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illo
                aliquam repellat molestias deserunt, neque vel.
              </p>
            </div>
            <div
              class="background--image"
              :style="{ backgroundImage: `url(${berlin})` }"
            ></div>
          </div> </splide-slide
        ><splide-slide>
          <div class="moscow city relative h-[550px] p-12">
            <div class="absolute bottom-8 left-8 text-white space-y-4">
              <a href="#">
                <span
                  class="
                    proporty__button
                    opacity-0
                    py-2
                    px-4
                    rounded-md
                    bg-c-blue
                    text-sm
                  "
                  >5 Proporties ></span
                >
              </a>
              <p class="font-semibold text-2xl">Moscow</p>
              <p class="text-sm w-4/5">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illo
                aliquam repellat molestias deserunt, neque vel.
              </p>
            </div>
            <div
              class="background--image"
              :style="{ backgroundImage: `url(${moscow})` }"
            ></div>
          </div>
        </splide-slide>
      </splide>
    </div>
  </div>
</template>

<script>
import paris from '~/assets/image/paris.jpg'
import berlin from '~/assets/image/berlin.jpg'
import moscow from '~/assets/image/moscow.jpg'
import amsterdam from '~/assets/image/amsterdam.jpg'
import newyork from '~/assets/image/newyork.jpg'

export default {
  data() {
    return {
      paris,
      berlin,
      moscow,
      amsterdam,
      newyork,
    }
  },
}
</script>

<style lang="scss" scoped>
.explore__title {
  position: relative;
  z-index: 1;
  .background--image {
    background-image: linear-gradient(
        to bottom,
        rgba(#073894, 1) 50%,
        rgba(transparent, 0)
      ),
      url('~/assets/image/blue-waves.jpg');
  }
}

.proporty__button {
  position: absolute;
  top: -30px;
  transform: translateY(-60px);

  transition: all 300ms ease-in-out;
}

.city {
  &:hover .proporty__button {
    opacity: 1;
    transform: translateY(0);
  }

  .background--image::before {
    content: '';
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    background-image: linear-gradient(
      to top,
      rgba(black, 0.5),
      rgba(black, 0) 30%
    );
  }
}

::v-deep .splide__pagination__page.is-active {
  background: white;
  transform: scale(1.6);
  opacity: 1;
}
</style>
