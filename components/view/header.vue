<template>
  <div>
    <div class="shadow-2xl relative z-10">
      <div class="header__top bg-black-light">
        <div
          class="grid grid-flow-col justify-end items-center gap-x-5 py-2 px-10"
        >
          <div class="space-x-2 divide-x-2 divide-gray-400">
            <span class="text-gray-300 text-sm">info@besideme.com </span>
            <span class="text-gray-300 text-sm pl-2">+90 545 55 55 </span>
          </div>
          <a
            href="#"
            class="
              px-4
              py-1
              bg-c-blue
              text-white
              rounded-md
              hover:bg-blue-800
              text-sm
              font-semibold
            "
            @click.stop="login = true"
            >Be a Partner</a
          >
        </div>
      </div>
      <div class="bg-gray-50">
        <div class="max-w-screen-xl mx-auto grid grid-flow-col justify-between">
          <ul
            class="nav grid grid-flow-col justify-start items-center gap-x-10"
          >
            <li>
              <a href="/"> <img src="/logo.png" alt="" class="h-10" /></a>
            </li>
            <li
              class="nav__item"
              @mouseenter="$event.target.classList.toggle('menu--open')"
              @mouseleave="$event.target.classList.toggle('menu--open')"
            >
              <a class="nav__link" href="#javascript"
                >Home
                <span class="menu-indicator">
                  <span class="menu-indicator-chevron"></span>
                </span>
              </a>
              <ul class="menu menu--main">
                <li><nuxt-link to="/property">Lorem</nuxt-link></li>
                <li><nuxt-link to="/property">Sit Ametes Cezete</nuxt-link></li>
                <li><nuxt-link to="/property">Valis Kaste Akse</nuxt-link></li>
                <li><nuxt-link to="/property">Mahtel Lerste</nuxt-link></li>
                <li><nuxt-link to="/property">Velse Kesente</nuxt-link></li>
                <li
                  class="nav__item"
                  @mouseenter="$event.target.classList.toggle('menu--open')"
                  @mouseleave="$event.target.classList.toggle('menu--open')"
                >
                  <a href="#javascript">
                    <div class="relative inline-block">
                      Sit Antenkentest
                      <span class="submenu-indicator">
                        <span class="submenu-indicator-chevron"></span>
                      </span>
                    </div>
                  </a>
                  <ul class="menu menu--sub">
                    <li><nuxt-link to="/property">Lorem Lore</nuxt-link></li>
                    <li><nuxt-link to="/property">Kalbe</nuxt-link></li>
                  </ul>
                </li>
              </ul>
            </li>
            <li
              class="nav__item"
              @mouseenter="$event.target.classList.toggle('menu--open')"
              @mouseleave="$event.target.classList.toggle('menu--open')"
            >
              <a class="nav__link" href="#"
                >Features
                <span class="menu-indicator">
                  <span class="menu-indicator-chevron"></span>
                </span>
              </a>
              <ul class="menu menu--main">
                <li
                  class="nav__item"
                  @mouseenter="$event.target.classList.toggle('menu--open')"
                  @mouseleave="$event.target.classList.toggle('menu--open')"
                >
                  <a href="">
                    <div class="relative inline-block">
                      Parsel
                      <span class="submenu-indicator">
                        <span class="submenu-indicator-chevron"></span>
                      </span>
                    </div>
                  </a>
                  <ul class="menu menu--sub">
                    <li><nuxt-link to="/property">Coffe</nuxt-link></li>
                    <li><nuxt-link to="/property">Coffe Tables</nuxt-link></li>
                    <li><nuxt-link to="/property">Tea Tea</nuxt-link></li>
                    <li><nuxt-link to="/property">Cold Tea</nuxt-link></li>
                  </ul>
                </li>
                <li
                  class="nav__item"
                  @mouseenter="$event.target.classList.toggle('menu--open')"
                  @mouseleave="$event.target.classList.toggle('menu--open')"
                >
                  <a href="">
                    <div class="relative inline-block">
                      Parsel Out
                      <span class="submenu-indicator">
                        <span class="submenu-indicator-chevron"></span>
                      </span>
                    </div>
                  </a>
                  <ul class="menu menu--sub">
                    <li><a href="">Lorem Itsum</a></li>
                    <li><a href="">Dolar Sit Amet</a></li>
                    <li><a href="">Braven</a></li>
                  </ul>
                </li>
                <li
                  class="nav__item"
                  @mouseenter="$event.target.classList.toggle('menu--open')"
                  @mouseleave="$event.target.classList.toggle('menu--open')"
                >
                  <a href="">
                    <div class="relative inline-block">
                      All the Things
                      <span class="submenu-indicator">
                        <span class="submenu-indicator-chevron"></span>
                      </span>
                    </div>
                  </a>
                  <ul class="menu menu--sub">
                    <li><a href="">Team A</a></li>
                    <li><a href="">Team B</a></li>
                  </ul>
                </li>
              </ul>
            </li>
            <li
              class="nav__item"
              @mouseenter="$event.target.classList.toggle('menu--open')"
              @mouseleave="$event.target.classList.toggle('menu--open')"
            >
              <a class="nav__link" href="#"
                >Projects
                <span class="menu-indicator">
                  <span class="menu-indicator-chevron"></span>
                </span>
              </a>
              <ul class="menu menu--main">
                <li><a href="#">Losta</a></li>
                <li><a href="">Sit Amete</a></li>
                <li><a href="">Valid By Goverment</a></li>
                <li
                  class="nav__item"
                  @mouseenter="$event.target.classList.toggle('menu--open')"
                  @mouseleave="$event.target.classList.toggle('menu--open')"
                >
                  <a href="">
                    <div class="relative inline-block">
                      Completed
                      <span class="submenu-indicator">
                        <span class="submenu-indicator-chevron"></span>
                      </span>
                    </div>
                  </a>
                  <ul class="menu menu--sub">
                    <li><a href="">Lorem Lore</a></li>
                    <li><a href="">Kalbe</a></li>
                  </ul>
                </li>
              </ul>
            </li>
            <li
              class="nav__item"
              @mouseenter="$event.target.classList.toggle('menu--open')"
              @mouseleave="$event.target.classList.toggle('menu--open')"
            >
              <a class="nav__link" href="#"
                >Pages
                <span class="menu-indicator">
                  <span class="menu-indicator-chevron"></span>
                </span>
              </a>
              <ul class="menu menu--main">
                <li><a href="#">Page A</a></li>
                <li><a href="">Example Page</a></li>
                <li><a href="">Solid</a></li>
              </ul>
            </li>
            <li>
              <a href="#" class="py-[30px] text-yellow-600">
                <font-awesome-icon
                  :icon="['fas', 'fire-alt']"
                  class="text-sm"
                ></font-awesome-icon>
                <span>New Proporties</span>
              </a>
            </li>
          </ul>
          <div class="grid grid-flow-col items-center gap-x-4">
            <a href="#" class="text-green-500" @click.stop="showLogin = true">
              <font-awesome-icon
                :icon="['fas', 'plus-circle']"
                class="text-sm"
              ></font-awesome-icon>
              <span class="font-semibold" @click="login = true"
                >Add Property</span
              >
            </a>
            <a
              href="#"
              class="bg-blue-dark text-white p-4 rounded-md"
              @click.stop="login = true"
            >
              <font-awesome-icon :icon="['fas', 'user']"></font-awesome-icon>
              <span class="ml-2 font-semibold">Sign In</span>
            </a>
            <v-dialog v-model="login" width="640px ">
              <login @clicked:register="toggleLogReg"></login>
            </v-dialog>
            <v-dialog v-model="register" width="1024px ">
              <register @clicked:login="toggleLogReg"></register>
            </v-dialog>
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
      register: false,
      login: false,
      itemOneActive: false,
      itemTwoActive: false,
      itemThreeActive: false,
      itemFourActive: false,
      show: true,
    }
  },
  methods: {
    toggleLogReg() {
      this.register = !this.register
      this.login = !this.login
    },
  },
}
</script>

<style lang="scss" scoped>
.nav {
  position: relative;
  z-index: 100;
}

.nav__item {
  position: relative;
  > .nav__link {
    padding: 30px 12px;
    font-weight: 500;
  }

  a {
    position: relative;
    display: inline-block;
    color: var(--black-dark);
    &:hover {
      @apply text-green-600;

      .menu-indicator-chevron {
        border-color: rgb(5, 150, 105);
      }
    }
  }
}

.menu {
  position: absolute;
  visibility: hidden;
  opacity: 0;
  transition: all 500ms;
  width: 240px;
  padding: 1rem;
  padding-bottom: 0;
  box-shadow: 0 0 50px 0 rgb(32 32 32 / 25%);
  @apply bg-gray-100 divide-y-2 rounded-md;

  &--main {
    &::before {
      background-color: inherit;
      content: '';
      height: 20px;
      left: 25px;
      position: absolute;
      top: -10px;
      -webkit-transform: rotate(45deg);
      -moz-transform: rotate(45deg);
      -o-transform: rotate(45deg);
      transform: rotate(45deg);
      width: 20px;
    }
  }

  &--sub {
    left: 100%;
    top: 0;
  }

  > li {
    padding: 14px;
  }

  a {
    width: 100%;
    &:hover {
      transform: translate(10px);
      @apply text-green-600;
      .submenu-indicator-chevron {
        border-color: green;
      }
    }
  }
}

.nav__item.menu--open {
  > .menu {
    display: block;
    visibility: visible;
    opacity: 1;
  }
}

.menu-indicator {
  position: absolute;
  top: 42%;
  right: 0;
  &-chevron {
    height: 6px;
    width: 6px;
    display: block;
    border-style: solid;
    border-width: 0 1px 1px 0;
    border-color: transparent var(--black-light) var(--black-light) transparent;
    transform: rotate(45deg);
  }
}
.submenu-indicator {
  position: absolute;
  top: 10px;
  left: 100%;
  margin-left: 5px;
  &-chevron {
    height: 6px;
    width: 6px;
    display: block;
    border-style: solid;
    border-width: 0 1px 1px 0;
    border-color: transparent #39466d #39466d transparent;
    transform: rotate(-45deg);
  }
}
</style>
