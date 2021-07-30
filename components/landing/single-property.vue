<template>
  <div
    class="property bg-white rounded-xl overflow-hidden w-full max-w-[420px]"
  >
    <div class="property__slide h-60">
      <splide
        :options="{
          rewind: true,
          perPage: 1,
          arrows: true,
          height: 240,
          pagination: false,
        }"
      >
        <splide-slide v-for="imageNo in property.images" :key="imageNo">
          <img
            class="w-full h-[240px] object-cover object-center"
            :src="`/images/home-${imageNo}.jpg`"
            alt=""
          />
        </splide-slide>
      </splide>
    </div>
    <div class="property__content py-4 space-y-4">
      <div class="flex items-center px-6">
        <div class="flex-1">
          <p class="text-gray-500 text-sm">{{ property.type }}</p>
          <p class="font-semibold text-gray-800">{{ property.title }}</p>
        </div>
        <span class="price text-c-blue font-bold text-lg">{{
          property.price.toLocaleString()
        }}</span>
      </div>
      <div class="px-6">
        <div class="flex text-gray-500 text-sm space-x-5">
          <div>
            <v-icon
              color="#a1abc9"
              size="1rem"
              class="bg-[#edf1f9] rounded-full p-1 inline-block"
            >
              mdi-bed-king-outline
            </v-icon>
            <span>{{ property.rooms }} Rooms</span>
          </div>
          <div>
            <v-icon
              color="#a1abc9"
              size=".9rem"
              class="bg-[#edf1f9] rounded-full p-1 inline-block"
              >mdi-axis-arrow</v-icon
            >

            <span>{{ property.sqrmtr }} sqrmtr</span>
          </div>
          <div>
            <v-icon
              color="#a1abc9"
              size="1rem"
              class="bg-[#edf1f9] rounded-full p-1 inline-block"
            >
              mdi-home-variant-outline
            </v-icon>
            <span> {{ property.age }} Age</span>
          </div>
        </div>
      </div>
      <div class="flex pt-4 px-6" style="border-top: 1px solid #e4e8f3">
        <div class="flex-1 flex items-center">
          <v-icon
            color="#a1abc9"
            size="1.3rem"
            class="rounded-full p-1 inline-block"
            >mdi-map-marker-outline
          </v-icon>
          <p class="text-gray-500">{{ property.shortAdress }}</p>
        </div>
        <a
          href="#javascript"
          class="bg-green-500 text-white text-sm px-2 py-1 rounded-2xl"
          >See More</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    property: {
      type: Object,
      default: () => {},
    },
  },
}
</script>

<style lang="scss" scoped>
.price::after {
  content: '\20BA';
  margin-left: 4px;
}

::v-deep .splide__arrow {
  background: rgba(255, 255, 255, 0.2);
  opacity: 0;

  transition: all 300ms ease-in-out;

  svg {
    fill: white;
  }
}

::v-deep .property__slide:hover .splide__arrow {
  opacity: 1;
}
</style>
