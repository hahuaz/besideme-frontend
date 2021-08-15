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
    <section class="bg-blue-50">
      <div class="max-w-screen-xl mx-auto">
        <div class="container mx-auto pt-48">
          <div
            class="
              w-4/6
              bg-white
              mx-auto
              absolute
              -top-24
              z-10
              rounded-md
              flex
              items-center
            "
          >
            <img
              src="/images/mini-home.png"
              class="p-8 m-8 bg-blue-50"
              alt=""
            />
            <div class="flex flex-col gap-2 items-baseline">
              <span
                class="
                  bg-yellow-200 bg-opacity-40
                  text-yellow-600
                  font-semibold
                  px-2
                  py-1
                  rounded-lg
                "
                >Rent</span
              >
              <p class="font-bold text-2xl">Cracilo Village</p>
              <div class="flex">
                <v-icon small>mdi-map-marker-outline </v-icon>
                <p class="font-thin text-gray-500">3599 Huntz Lane View</p>
              </div>
              <span class="text-3xl font-bold text-green-500"
                >$3,244
                <span class="font-thin text-gray-500 text-base"
                  >/monthly</span
                ></span
              >
              <div
                class="flex text-gray-500 text-sm space-x-5 mt-2 items-center"
              >
                <div>
                  <v-icon
                    color="#a1abc9"
                    size="1rem"
                    class="bg-[#edf1f9] rounded-full p-1 inline-block"
                  >
                    mdi-bed-king-outline
                  </v-icon>
                  <span>3 Rooms</span>
                </div>
                <div>
                  <v-icon
                    color="#a1abc9"
                    size=".9rem"
                    class="bg-[#edf1f9] rounded-full p-1 inline-block"
                    >mdi-axis-arrow</v-icon
                  >

                  <span>232 sqrmtr</span>
                </div>
                <div>
                  <v-icon
                    color="#a1abc9"
                    size="1rem"
                    class="bg-[#edf1f9] rounded-full p-1 inline-block"
                  >
                    mdi-home-variant-outline
                  </v-icon>
                  <span> 5 Age</span>
                </div>
              </div>
            </div>
          </div>
          <div class="flex gap-8">
            <v-expansion-panels :value="1" class="" popout>
              <v-expansion-panel>
                <v-expansion-panel-header>
                  <span class="font-bold text-xl" style="flex: unset"
                    >Details About Property</span
                  >
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  <div class="grid grid-cols-3 gap-4">
                    <div>
                      <span class="font-semibold">Parent Bedroom:</span>
                      <span>Yes</span>
                    </div>
                    <div>
                      <span class="font-semibold">Garage:</span>
                      <span>&#10003; </span>
                    </div>
                    <div>
                      <span class="font-semibold">Elevator:</span>
                      <span>&#10003; </span>
                    </div>
                    <div>
                      <span class="font-semibold">Garden:</span>
                      <span>30 sqrmtr </span>
                    </div>
                  </div>
                </v-expansion-panel-content>
              </v-expansion-panel>
              <v-expansion-panel>
                <v-expansion-panel-header>
                  <span class="font-bold text-xl" style="flex: unset"
                    >Description</span
                  >
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  <div class="grid grid-cols-3 gap-4">
                    <p>
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Porro eum, error magnam et ipsam dolor unde commodi
                      numquam fugiat reprehenderit nostrum iusto exercitationem
                      blanditiis dicta provident minus officiis dolore id.
                    </p>
                    <p>
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Porro eum, error magnam et ipsam dolor unde commodi
                      numquam fugiat reprehenderit nostrum iusto...
                    </p>
                    <p>
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                      Porro eum, error magnam et ipsam.
                    </p>
                  </div>
                </v-expansion-panel-content>
              </v-expansion-panel>
              <v-expansion-panel>
                <v-expansion-panel-header>
                  <span class="font-bold text-xl" style="flex: unset"
                    >Property Video</span
                  >
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                  <div class="w-full h-96 relative">
                    <img
                      src="/images/video-placeholder.png"
                      class="w-full h-full object-center object-cover"
                      alt=""
                    />
                  </div>
                </v-expansion-panel-content>
              </v-expansion-panel>
            </v-expansion-panels>
            <div
              class="
                w-64
                bg-white
                flex flex-col
                justify-center
                items-center
                gap-4
                px-4
                py-8
                self-start
                rounded-md
              "
            >
              <v-btn outlined block x-large color="#dd8622">
                &#9829; Save</v-btn
              >

              <v-btn outlined block x-large color="#10b981">
                &#x02937; Share</v-btn
              >
              <v-btn style="color: white" block x-large color="#10b981">
                <v-icon> mdi-phone</v-icon> CALL THE AGENT</v-btn
              >
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-blue-50">
      <div class="max-w-screen-xl mx-auto py-24">
        <div class="image-grid container mx-auto px-4">
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
