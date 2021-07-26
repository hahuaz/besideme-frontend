<template>
  <footer>
    <div>
      <div class="footer-middle bg-black-light py-12">
        <div class="max-w-screen-xl mx-auto">
          <div class="container">
            <div class="">
              <div class="space-y-4 text-blue-100">
                <img src="/logo.png" alt="" />
                <p>Popaya Street West, Aloha 8007, Turkey.</p>
                <p>+90 246-345-0695</p>
                <p>info@example.com</p>
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
                <li><a href="#"> Company Details </a></li>
                <li><a href="#"> Assets </a></li>
              </ul>
            </div>
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
