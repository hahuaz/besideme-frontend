<template>
  <div
    ref="counts"
    class="counts__container grid grid-cols-4 justify-around items-center py-32"
  >
    <div class="count">
      <v-icon color="#1266e3" size="5rem" class="count__icon">
        mdi-chart-pie</v-icon
      >
      <div class="count__value">
        <span id="dominance" class="w-10">11</span>
        <span>%</span>
      </div>
      <p class="count__type">Marketplace Holding</p>
    </div>
    <div class="count">
      <v-icon color="#1266e3" class="count__icon" size="5rem">
        mdi-account-group</v-icon
      >
      <div class="count__value">
        <span id="client" class="w-14">119</span> <span>+</span>
      </div>
      <p class="count__type">Client Around The World</p>
    </div>
    <div class="count">
      <v-icon color="#1266e3" class="count__icon" size="5rem">
        mdi-home-analytics</v-icon
      >
      <div class="count__value">
        <span id="house" class="w-14">121</span> <span>+</span>
      </div>
      <p class="count__type">Sold Hosue</p>
    </div>
    <div class="count">
      <v-icon color="#1266e3" class="count__icon" size="5rem">
        mdi-chart-timeline-variant-shimmer</v-icon
      >
      <div class="count__value">
        <span id="growth" class="w-10">13</span> <span>%</span>
      </div>
      <p class="count__type">Market Growth</p>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    const observer = new IntersectionObserver(this.animate, {
      threshold: 1,
      root: null,
    })
    observer.observe(this.$refs.counts)
  },

  methods: {
    animate(entries, observer) {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          /* start the animations */
          const gsap = this.$gsap

          /* dominance */
          const dominance = { val: 11 }
          gsap.to(dominance, 5, {
            val: 74,
            roundProps: 'val',
            onUpdate() {
              document.getElementById('dominance').textContent = dominance.val
            },
          })

          /* client */
          const client = { val: 119 }
          gsap.to(client, 5, {
            val: 285,
            roundProps: 'val',
            onUpdate() {
              document.getElementById('client').textContent = client.val
            },
          })

          /* client */
          const house = { val: 121 }
          gsap.to(house, 5, {
            val: 641,
            roundProps: 'val',
            onUpdate() {
              document.getElementById('house').textContent = house.val
            },
          })

          /* growth */
          const growth = { val: 13 }
          gsap.to(growth, 5, {
            val: 19,
            roundProps: 'val',
            onUpdate() {
              document.getElementById('growth').textContent = growth.val
            },
          })
        }
      })
    },
  },
}
</script>

<style lang="scss" scoped>
.counts__container {
  .count {
    text-align: center;
  }
  .count__value {
    @apply text-4xl font-extrabold my-4 relative;
    span {
      display: inline-block;
    }
  }
  .count__type {
    @apply text-gray-500 font-semibold;
  }
}
</style>
