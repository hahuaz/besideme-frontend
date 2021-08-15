<template>
  <div>
    <div class="head-carousel">
      <splide
        :options="{
          rewind: true,
          perPage: 2,
          arrows: true,
          height: 600,
          pagination: false,
        }"
      >
        <splide-slide v-for="imageNo in 9" :key="imageNo">
          <img
            class="w-full h-full object-cover object-center"
            :src="`/images/home-${imageNo}.jpg`"
            alt=""
          />
        </splide-slide>
      </splide>
    </div>
    <section>
      <div class="max-w-screen-xl mx-auto">
        <div class="image-grid container mx-auto py-12 px-4">
          <div class="a1">
            <img
              class="w-full h-full object-cover object-center"
              src="/images/home-1.jpg"
              alt=""
            />
          </div>
          <div class="a2">
            <img
              class="w-full h-full object-cover object-center"
              src="/images/home-2.jpg"
              alt=""
            />
          </div>
          <div class="a3">
            <img
              class="w-full h-full object-cover object-center"
              src="/images/home-3.jpg"
              alt=""
            />
          </div>
          <div class="a4">
            <img
              class="w-full h-full object-cover object-center"
              src="/images/home-4.jpg"
              alt=""
            />
          </div>
          <div class="a5">
            <img
              class="w-full h-full object-cover object-center"
              src="/images/home-5.jpg"
              alt=""
            />
          </div>
          <div class="a6">
            <img
              class="w-full h-full object-cover object-center"
              src="/images/home-6.jpg"
              alt=""
            />
          </div>
          <div class="a7">
            <img
              class="w-full h-full object-cover object-center"
              src="/images/home-7.jpg"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {}
</script>
<style lang="scss">
.head-carousel {
  .splide__arrow--next {
    right: 2rem;
  }
  .splide__arrow--prev {
    left: 2rem;
  }
  .splide__arrow {
    background: white;
    opacity: 1;
    height: 2.5rem;
    width: 2.5rem;
    fill: rgb(0, 197, 0);
  }
}
</style>

<style lang="scss" scoped>
.image-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr 1fr;
  grid-auto-rows: 5vw;
  gap: 20px 20px;
  grid-auto-flow: row;
  grid-template-areas:
    '. a1 a1 a1 a1 a1 a2 a2 a2 . . .'
    '. a1 a1 a1 a1 a1 a2 a2 a2 a3 a3 .'
    '. a1 a1 a1 a1 a1 a2 a2 a2 a3 a3 .'
    '. a1 a1 a1 a1 a1 a4 a4 a4 a4 a4 a4'
    'a5 a5 a5 a5 a5 a5 a4 a4 a4 a4 a4 a4'
    'a5 a5 a5 a5 a5 a5 a4 a4 a4 a4 a4 a4'
    'a5 a5 a5 a5 a5 a5 a4 a4 a4 a4 a4 a4'
    'a5 a5 a5 a5 a5 a5 a4 a4 a4 a4 a4 a4'
    '. . . a6 a6 a6 a7 a7 a7 a7 . .'
    '. . . a6 a6 a6 a7 a7 a7 a7 . .'
    '. . . a6 a6 a6 a7 a7 a7 a7 . .'
    '. . . . . . a7 a7 a7 a7 . .';
}

.a1 {
  grid-area: a1;
}

.a2 {
  grid-area: a2;
}

.a3 {
  grid-area: a3;
}

.a4 {
  grid-area: a4;
}

.a5 {
  grid-area: a5;
}

.a6 {
  grid-area: a6;
}

.a7 {
  grid-area: a7;
}
</style>
