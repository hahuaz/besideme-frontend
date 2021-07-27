<template>
  <div>
    <section>
      <div class="background--wrapper">
        <div class="max-w-screen-xl mx-auto">
          <div class="container">
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
        <div class="background--image"></div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      keywords: null,
      minprice: null,
      paxprice: null,
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

.background--image {
  background-image: linear-gradient(to bottom, rgba(gray, 0.3), rgba(gray, 0.3)),
    url('~/assets/image/landing-hero.jpg');
}
</style>
