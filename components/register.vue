<template>
  <div>
    <div class="max-w-screen-lg bg-white">
      <div class="text-blue-dark text-center font-extrabold text-6xl py-8">
        Registration
      </div>
      <div class="px-24 text-center">
        <div class="grid grid-cols-2 gap-x-4">
          <v-text-field
            v-model="firstname"
            background-color="#eff6ff"
            color="#1266e3"
            filled
            label="First Name"
            prepend-inner-icon="mdi-account-outline"
          ></v-text-field>
          <v-text-field
            v-model="lastname"
            background-color="#eff6ff"
            color="#1266e3"
            filled
            label="Last Name"
            prepend-inner-icon="mdi-account-outline"
          ></v-text-field>
          <v-text-field
            v-model="email"
            background-color="#eff6ff"
            color="#1266e3"
            filled
            label="Email"
            prepend-inner-icon="mdi-email-outline"
          ></v-text-field>
          <v-text-field
            v-model="password"
            type="password"
            background-color="#eff6ff"
            color="#1266e3"
            filled
            counter="25"
            hint="Password's length can only be 25."
            label="Password"
            prepend-inner-icon="mdi-lock-outline"
          ></v-text-field>
        </div>

        <div class="flex justify-center mb-4">
          <v-checkbox
            v-model="terms"
            dense
            color="#1266e3"
            hide-details
          ></v-checkbox>
          <span class="relative top-[6px] ml-1"
            >I have read
            <a href="#javascript" class="text-c-blue">Terms and conditions</a>
            .</span
          >
        </div>
        <a
          href="#javascript"
          class="
            text-center
            inline-block
            py-4
            px-48
            rounded-full
            bg-c-blue
            text-white text-lg
          "
          >Register</a
        >
        <div class="grid grid-flow-row justify-items-center py-6 space-y-4">
          <div>
            Already have an account?
            <span
              class="cursor-pointer text-yellow-600"
              @click="$emit('clicked:login')"
              >Login.</span
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      firstname: null,
      lastname: null,
      email: null,
      password: null,
      terms: false,
    }
  },
}
</script>

<style lang="scss" scoped></style>
