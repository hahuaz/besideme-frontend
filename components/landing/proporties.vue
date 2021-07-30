<template>
  <div>
    <div class="py-24">
      <div class="proporties__header text-center max-w-xl mx-auto space-y-4">
        <p class="text-blue-dark font-bold text-4xl">
          Proporties On The Market
        </p>
        <p class="text-gray-500 text-sm">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cum facere
          inventore in repudiandae. Facere amet fuga veritatis cumque nisi
          minima est accusant.
        </p>
      </div>
      <div
        class="
          grid grid-cols-1
          md:grid-cols-2
          lg:grid-cols-3
          place-items-center
          gap-6
          pt-10
          pb-6
          px-4
        "
      >
        <landing-single-property
          v-for="(veri, i) in properties"
          :key="i"
          :property="veri"
        ></landing-single-property>
      </div>
      <div class="text-center">
        <a
          href="#javascript"
          class="
            py-4
            px-6
            bg-green-50
            border-2 border-green-400
            text-green-500
            inline-block
            rounded-md
            font-semibold
          "
        >
          SEE MORE HOUSES
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      properties: [
        {
          images: [1, 8, 9],
          type: 'Rent',
          title: 'Vinchester Village',
          price: 3400,
          rooms: 3,
          sqrmtr: 154,
          age: 5,
          shortAdress: 'Vanilla Street',
        },
        {
          images: [2, 7, 6],
          type: 'Sell',
          title: 'Luxry Vİllage',
          price: 119700,
          rooms: 4,
          sqrmtr: 254,
          age: 1,
          shortAdress: 'Nanely Street',
        },
        {
          images: [3, 5, 4],
          type: 'Rent',
          title: 'Sims Village',
          price: 2300,
          rooms: 2,
          sqrmtr: 134,
          age: 2,
          shortAdress: 'Kalsib Avenue',
        },
        {
          images: [4, 1, 2],
          type: 'Buy',
          title: 'Vinchester Apartment',
          price: 333400,
          rooms: 2,
          sqrmtr: 54,
          age: 6,
          shortAdress: 'Depsen Avenue',
        },
        {
          images: [5, 3, 2],
          type: 'Rent',
          title: 'Kalibre Real Estate',
          price: 1200,
          rooms: 3,
          sqrmtr: 114,
          age: 5,
          shortAdress: 'Vanilla Alk Area',
        },
        {
          images: [6, 1, 2],
          type: 'Rent',
          title: 'Besideme Aparment',
          price: 1400,
          rooms: 3,
          sqrmtr: 154,
          age: 5,
          shortAdress: 'Debulve District',
        },
        {
          images: [7, 3, 4],
          type: 'Rent',
          title: 'Palas Home',
          price: 2400,
          rooms: 3,
          sqrmtr: 154,
          age: 5,
          shortAdress: 'Vanilla Street',
        },
        {
          images: [8, 4, 5],
          type: 'Rent',
          title: 'Brown Village',
          price: 5400,
          rooms: 5,
          sqrmtr: 194,
          age: 9,
          shortAdress: 'Sarsal District',
        },
        {
          images: [9, 6, 1],
          type: 'Buy',
          title: 'Vinchester Village',
          price: 133400,
          rooms: 2,
          sqrmtr: 164,
          age: 0,
          shortAdress: 'Kalben District',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped></style>
