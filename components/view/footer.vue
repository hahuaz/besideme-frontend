<template>
  <footer>
    <div class="footer-top bg-c-blue">
      <div class="max-w-screen-xl mx-auto">
        <div class="container">
          <div class="grid grid-flow-col justify-between items-center h-40">
            <div class="text-gray-50 font-serif">
              <p class="text-2xl font-bold">
                Want To Work With A Real Estate Agent?
              </p>
              <p class="text-lg">
                We'll help you to grow your career and assets.
              </p>
            </div>
            <div>
              <a
                href="#"
                class="
                  py-6
                  px-12
                  rounded-full
                  bg-gray-100
                  text-gray-600
                  font-semibold
                  border-4 border-blue-300
                "
              >
                Contact Now
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-middle bg-black-light py-12">
      <div class="max-w-screen-xl mx-auto">
        <div class="container">
          <div class="">
            <div class="space-y-4 text-blue-100">
              <img src="/logo.png" alt="" />
              <p>Popaya Street West, Aloha 8007, Turkey.</p>
              <p>+90 246-345-0695</p>
              <p>info@example.com</p>
              <div class="pt-4 w-52">
                <ul class="footer-bottom-social grid grid-flow-col gap-x-6">
                  <li>
                    <a href="https://www.facebook.com/">
                      <font-awesome-icon
                        class="icon"
                        :icon="['fab', 'facebook-f']"
                      />
                    </a>
                  </li>
                  <li>
                    <a href="https://www.twitter.com/">
                      <font-awesome-icon
                        class="icon"
                        :icon="['fab', 'twitter']"
                      />
                    </a>
                  </li>
                  <li>
                    <a href="https://www.instagram.com/">
                      <font-awesome-icon
                        class="icon"
                        :icon="['fab', 'instagram']"
                      />
                    </a>
                  </li>
                  <li>
                    <a href="https://www.linkedin.com/">
                      <font-awesome-icon
                        class="icon"
                        :icon="['fab', 'linkedin-in']"
                      />
                    </a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <div>
            <ul class="grid gap-y-2">
              <h1 class="pb-2">Navigations</h1>
              <li><a href="#"> About Us </a></li>
              <li><a href="#"> FAQs </a></li>
              <li><a href="#"> Contact </a></li>
              <li><a href="#"> Blog </a></li>
            </ul>
          </div>
          <div>
            <ul class="grid gap-y-2">
              <h1 class="pb-2">The Highlights</h1>
              <li><a href="#"> Apartment </a></li>
              <li><a href="#"> Houses </a></li>
              <li><a href="#"> Villas </a></li>
              <li><a href="#"> By Sea </a></li>
            </ul>
          </div>
          <div>
            <ul class="grid gap-y-2">
              <h1 class="pb-2">Agent & Company</h1>
              <li><a href="#"> Company Details </a></li>
              <li><a href="#"> Assets </a></li>
              <li><a href="#"> Our History </a></li>
              <li><a href="#"> Our Partners </a></li>
            </ul>
          </div>
          <div>
            <ul class="grid gap-y-2">
              <h1 class="pb-2">Download Apps</h1>
              <li>
                <a href="#">
                  <div
                    class="
                      border-2 border-gray-600
                      rounded-md
                      grid grid-flow-col
                      gap-x-4
                      justify-start
                      items-center
                      px-4
                      py-3
                    "
                  >
                    <font-awesome-icon
                      :icon="['fab', 'apple']"
                      class="text-6xl text-c-blue"
                    ></font-awesome-icon>
                    <div>
                      <p class="text-white text-lg">App Store</p>
                      <p class="text-gray-400 text-sm">Get It Now</p>
                    </div>
                  </div>
                </a>
              </li>
              <li>
                <a href="#">
                  <div
                    class="
                      border-2 border-gray-600
                      rounded-md
                      grid grid-flow-col
                      gap-x-4
                      justify-start
                      items-center
                      px-4
                      py-3
                    "
                  >
                    <font-awesome-icon
                      :icon="['fab', 'google-play']"
                      class="text-5xl text-c-blue"
                    ></font-awesome-icon>
                    <div>
                      <p class="text-white text-lg">Google Play</p>
                      <p class="text-gray-400 text-sm">Get It Now</p>
                    </div>
                  </div>
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-bottom bg-black-dark py-6">
      <div class="max-w-screen-xl mx-auto">
        <div class="container">
          <div class="text-blue-100 grid grid-flow-col justify-around">
            <div>
              <p>© 2021 Besideme.com - All rights reserved by <i>Hahuaz</i>.</p>
            </div>
            <div>
              <a href="#">Terms of use </a>
              <a href="#" class="ml-4">Privaciy Policy </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.footer-middle {
  h1 {
    color: white;
    font-weight: 500;
  }
  a {
    @apply text-blue-100;
    &:hover {
      color: white;
    }
  }
  .container {
    display: grid;
    grid-template-columns: 1.5fr 1fr 1fr 1fr 1.5fr;
  }
}

.footer-bottom-social {
  .icon {
    transition: all 300ms linear;
    font-size: 1.4rem;
    &:hover {
      color: white;
      transform: scale(1.1);
    }
  }
}
</style>
