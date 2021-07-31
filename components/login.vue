<template>
  <div>
    <div class="max-w-screen-sm bg-white">
      <div class="text-blue-dark text-center font-extrabold text-6xl py-8">
        Log <span class="text-c-blue">In</span>
      </div>
      <div class="px-24">
        <v-text-field
          v-model="email"
          background-color="#eff6ff"
          color="#1266e3"
          filled
          label="E-mail"
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
        <a
          href="#javascript"
          class="
            text-center
            inline-block
            w-full
            py-4
            rounded-full
            bg-c-blue
            text-white text-lg
          "
          >Login</a
        >
        <div class="grid grid-flow-row justify-items-center py-6 space-y-4">
          <span class="inline-block cursor-pointer text-yellow-600"
            >Forget Password?</span
          >
          <div>
            Don't have an account?
            <span
              class="cursor-pointer text-yellow-600"
              @click="$emit('clicked:register')"
              >Register.</span
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
      email: null,
      password: null,
    }
  },
}
</script>

<style lang="scss" scoped></style>
