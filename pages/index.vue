<template>
  <div>
    <section class="hero">
      <div class="background--wrapper h-[850px]">
        <div class="max-w-screen-xl mx-auto">
          <div class="container mx-auto">
            <div class="p-24">
              <div class="hero-search max-w-lg px-8 py-12 bg-white rounded-md">
                <p class="text-4xl font-bold text-blue-900 mb-5">
                  Find Accessible Homes <br />
                  To Rent Or Buy
                </p>
                <div class="grid grid-cols-2 gap-4">
                  <div class="col-span-2">
                    <v-text-field
                      v-model="keywords"
                      color="#1266e3"
                      filled
                      background-color="#eff6ff"
                      label="Keywords..."
                      prepend-inner-icon="mdi-map-marker"
                      hide-details
                    ></v-text-field>
                  </div>
                  <div>
                    <v-select
                      v-model="minprice"
                      background-color="#eff6ff"
                      filled
                      :items="['500', '1000', '5000']"
                      :menu-props="{ bottom: true, offsetY: true }"
                      label="Min Price"
                      color="#1266e3"
                      hide-details
                    ></v-select>
                  </div>
                  <div>
                    <v-select
                      v-model="maxprice"
                      background-color="#eff6ff"
                      filled
                      :items="['10000', '20000', '30000']"
                      :menu-props="{ bottom: true, offsetY: true }"
                      label="Max Price"
                      color="#1266e3"
                      hide-details
                    ></v-select>
                  </div>
                  <div>
                    <v-select
                      v-model="type"
                      background-color="#eff6ff"
                      filled
                      :items="['Apartment', 'Office', 'Villa']"
                      :menu-props="{ bottom: true, offsetY: true }"
                      label="Property Type"
                      color="#1266e3"
                      hide-details
                    ></v-select>
                  </div>
                  <div>
                    <v-select
                      v-model="rooms"
                      background-color="#eff6ff"
                      filled
                      :items="['2', '3', '4']"
                      :menu-props="{ bottom: true, offsetY: true }"
                      label="Rooms"
                      color="#1266e3"
                      hide-details
                    ></v-select>
                  </div>
                  <div class="col-span-2">
                    <v-select
                      v-model="location"
                      background-color="#eff6ff"
                      filled
                      :items="[
                        'İstanbul - Turkey',
                        'Ankara - Turkey ',
                        'Berlin - Germany',
                        'London - UK',
                      ]"
                      :menu-props="{ bottom: true, offsetY: true }"
                      label="Location"
                      color="#1266e3"
                      hide-details
                    ></v-select>
                  </div>
                  <div class="col-span-2">
                    <v-btn block color="#1266e3" elevation="2" large x-large
                      >Search Result</v-btn
                    >
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="hero background--image"></div>
      </div>
    </section>
    <section class="about-us">
      <div class="py-24">
        <div class="max-w-screen-xl mx-auto">
          <div class="container mx-auto">
            <div class="grid grid-cols-2">
              <div class="relative">
                <div class="image__wrapper">
                  <img src="~/assets/image/landing-aboutus.png" alt="" />
                </div>
                <div class="absolute bottom-24 -left-6 z-10">
                  <div class="relative rounded-sm overflow-hidden">
                    <img
                      src="~/assets/image/gray-sofa-white-living-room-small.jpg"
                      alt=""
                      class="h-52 w-80"
                    />
                    <span
                      class="
                        absolute
                        top-1/2
                        left-1/2
                        transform
                        -translate-x-1/2 -translate-y-1/2
                        bg-white
                        rounded-full
                        p-4
                        pulse
                        cursor-pointer
                      "
                      @click.stop="dialog = true"
                    >
                      <v-icon large color="#ff5a3c"> mdi-play </v-icon>
                    </span>
                    <v-dialog v-model="dialog" width="600px">
                      <div class="">
                        <!-- TODO when you close the dialog without stopping video, video continous to play -->
                        <iframe
                          width="600"
                          height="500"
                          src="https://www.youtube.com/embed/7WkT4SmrzwE"
                          title="YouTube video player"
                          frameborder="0"
                          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                          allowfullscreen
                        ></iframe>
                      </div>
                    </v-dialog>
                  </div>
                </div>
              </div>
              <div class="py-12 space-y-6">
                <span
                  class="
                    bg-blue-100
                    px-4
                    py-1
                    text-blue-600
                    inline-block
                    rounded-xl
                  "
                  >About Us
                </span>
                <p class="font-bold text-5xl leading leading-snug">
                  Leader On The Real Estate Marketplace Area
                  <span
                    class="text-blue-600 text-7xl relative -left-4"
                    style="line-height: 0"
                    >.</span
                  >
                </p>
                <p class="text-gray-500 w-5/6 leading-normal">
                  Serve to 39,000 people which happy with us. Serve to more than
                  70 countries all over the world. Always eyes on the horizon.
                </p>
                <div class="text-gray-500 grid grid-cols-2 gap-y-8 py-4">
                  <div>
                    <v-icon color="#1266e3" class="p-2 bg-blue-100 rounded-full"
                      >mdi-heart-half-full</v-icon
                    >
                    <span class="ml-2">Loved by Customers </span>
                  </div>
                  <div>
                    <v-icon color="#1266e3" class="p-2 bg-blue-100 rounded-full"
                      >mdi-sprout</v-icon
                    >
                    <span class="ml-2">Always Trusted </span>
                  </div>
                  <div>
                    <v-icon color="#1266e3" class="p-2 bg-blue-100 rounded-full"
                      >mdi-certificate-outline</v-icon
                    >
                    <span class="ml-2">Exclusive Expriences </span>
                  </div>
                  <div>
                    <v-icon color="#1266e3" class="p-2 bg-blue-100 rounded-full"
                      >mdi-chart-bell-curve-cumulative</v-icon
                    >
                    <span class="ml-2">On The Top Of Chart </span>
                  </div>
                </div>
                <div class="p-6 border-l-4 border-c-blue bg-blue-100 w-4/6">
                  <p class="text-gray-500">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Aliquam, nisi aspernatur perspiciatis sit earum.
                  </p>
                </div>
                <a href="#" class="inline-block px-8 py-4 bg-c-blue text-white"
                  >Our History</a
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="explore">
      <div class="counter mx-auto mt-24">
        <landing-explore></landing-explore>
      </div>
    </section>
    <section class="business-count bg-blue-50">
      <div class="max-w-screen-xl mx-auto">
        <div class="counter mx-auto">
          <landing-counts></landing-counts>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
      keywords: null,
      minprice: null,
      maxprice: null,
      type: null,
      rooms: null,
      location: null,
    }
  },
}
</script>

<style lang="scss" scoped>
::v-deep .v-btn__content {
  color: white;
}

::v-deep .v-input__prepend-inner {
  margin-right: 6px;
}

.hero.background--image {
  background-image: linear-gradient(
      to bottom,
      rgba(black, 0.3),
      rgba(black, 0.3)
    ),
    url('~/assets/image/landing-hero.jpg');
}
</style>
