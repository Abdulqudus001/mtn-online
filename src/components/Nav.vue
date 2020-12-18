<template>
  <nav class="navbar container-fluid px-3 px-md-5 py-3">
    <ul class="row align-items-center mx-0">
      <li class="navbar__logo ml-0">
        <a href="/">
          <img src="../assets/logo.svg" alt="MTNNG logo image">
        </a>
      </li>
      <div
        class="nav__items row align-items-center"
        :class="active ? 'active' : 'not-active'"
      >
        <li
          @mouseover="openMenu('personal')"
          @mouseleave="openMenu('')"
          @click.prevent="openMenuClick('personal')"
        >
          <a href="#">
            Personal
            <i class="fa fa-angle-down ml-2"></i>
          </a>
          <ul v-if="currentMenu === 'personal'" class="sub-menu">
            <li
              class="mx-0"
              @mouseover="openSubMenu('services')"
              @mouseleave="openSubMenu('')"
            >
              <a href="#" class="mx-0 row justify-content-between align-items-center flex-nowrap">
                <span>
                  Services
                </span>
                <i class="fa fa-angle-right ml-4"></i>
              </a>
              <ul v-if="currentSubMenu === 'services'" class="sub-menu sub-menu--sub">
                <li class="mx-0">
                  <a href="#">
                    Tariff Plans
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Roaming
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    International Rates
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Country Code Prefix
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Recharge
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    SIM Services
                  </a>
                </li>
              </ul>
            </li>
            <li
              class="mx-0"
              @mouseover="openSubMenu('data')"
              @mouseleave="openSubMenu('')"
            >
              <a href="#" class="mx-0 row justify-content-between align-items-center flex-nowrap">
                <span>
                  Data
                </span>
                <i class="fa fa-angle-right ml-4"></i>
              </a>
              <ul v-if="currentSubMenu === 'data'" class="sub-menu sub-menu--sub">
                <li class="mx-0">
                  <a href="#">
                    Data Plans
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Social Media Bundles
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Video Streaming Pack
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Data Gifting
                  </a>
                </li>
              </ul>
            </li>
            <li
              class="mx-0"
              @mouseover="openSubMenu('devices')"
              @mouseleave="openSubMenu('')"
            >
              <a href="#" class="mx-0 row justify-content-between align-items-center flex-nowrap">
                <span>
                  Devices
                </span>
                <i class="fa fa-angle-right ml-4"></i>
              </a>
              <ul v-if="currentSubMenu === 'devices'" class="sub-menu sub-menu--sub">
                <li class="mx-0">
                  <a href="#">
                    Device Financing
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    4G MiFi
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Smart Feature Phone
                  </a>
                </li>
              </ul>
            </li>
            <li
              class="mx-0"
              @mouseover="openSubMenu('started')"
              @mouseleave="openSubMenu('')"
            >
              <a href="#" class="mx-0 row justify-content-between align-items-center flex-nowrap">
                <span>
                  Getting Started
                </span>
                <i class="fa fa-angle-right ml-4"></i>
              </a>
              <ul v-if="currentSubMenu === 'started'" class="sub-menu sub-menu--sub">
                <li class="mx-0">
                  <a href="#">
                    Coverage Map
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Find a store
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    How-to guides
                  </a>
                </li>
                <li class="mx-0">
                  <a href="#">
                    Internet settings
                  </a>
                </li>
              </ul>
            </li>
            <li class="mx-0">
              <a href="#">
                myMTN App
              </a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#">Business</a>
        </li>
        <li
          @mouseover="openMenu('investors')"
          @mouseleave="openMenu('')"
          @click.prevent="openMenuClick('investors')"
        >
          <a href="#">
            Investors
            <i class="fa fa-angle-down ml-2"></i>
          </a>
          <ul v-if="currentMenu === 'investors'" class="sub-menu">
            <li class="mx-0">
              <a href="#">
                More in Investors
              </a>
            </li>
            <li class="mx-0">
              <a href="#">
                Shareholders
              </a>
            </li>
            <li class="mx-0">
              <a href="#">
                Financial Reporting
              </a>
            </li>
            <li class="mx-0">
              <a href="#">
                Announcements
              </a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#">Foundation</a>
        </li>
        <li>
          <a href="#">Events</a>
        </li>
        <li
          @mouseover="openMenu('support')"
          @mouseleave="openMenu('')"
          @click.prevent="openMenuClick('support')"
        >
          <a href="#">
            Support
            <i class="fa fa-angle-down ml-2"></i>
          </a>
          <ul v-if="currentMenu === 'support'" class="sub-menu">
            <li class="mx-0">
              <a href="#">
                Help Center
              </a>
            </li>
            <li class="mx-0">
              <a href="#">
                Community
              </a>
            </li>
          </ul>
        </li>
        <li>
          <a href="#">About Us</a>
        </li>
        <li>
          <a href="#">Careers</a>
        </li>
        <li
          @mouseover="openMenu('contact')"
          @mouseleave="openMenu('')"
          @click.prevent="openMenuClick('contact')"
        >
          <a href="#">
            Contact Us
            <i class="fa fa-angle-down ml-2"></i>
          </a>
          <ul v-if="currentMenu === 'contact'" class="sub-menu">
            <li class="mx-0">
              <a href="#">
                MTN Supplier
              </a>
            </li>
          </ul>
        </li>
        <li class="d-lg-none">
          <div class="search-bar">
            <i class="fa fa-search"></i>
            <input type="search" placeholder="Search...">
          </div>
        </li>
      </div>
    </ul>
    <div class="search-bar d-none d-lg-block">
      <i class="fa fa-search"></i>
      <input type="search" placeholder="Search...">
    </div>
    <button
      class="hamburger d-lg-none"
      :class="active ? 'active' : 'not-active'"
      @click="active = !active"
    >
      <span></span>
      <span></span>
      <span></span>
    </button>
  </nav>
</template>

<script>
export default {
  data: () => ({
    active: false,
    currentMenu: '',
    currentSubMenu: '',
  }),
  methods: {
    openMenuClick(name) {
      if (window.innerWidth < 992) {
        if (this.currentMenu === name) {
          this.currentMenu = '';
        } else {
          this.currentMenu = name;
        }
      }
    },
    openMenu(name) {
      if (window.innerWidth >= 992) {
        this.currentMenu = name;
      }
    },
    openSubMenu(name) {
      if (window.innerWidth >= 992) {
        this.currentSubMenu = name;
      }
    },
  },
};
</script>

<style lang="scss" scoped>
.navbar {
  background-color: #FFCC00;
  color: #000;
  width: 100vw;

  &__logo img {
    width: 40px;
  }

  ul {
    list-style-type: none;
    padding-left: 0;
    margin-bottom: 0;

    li {
      margin: 0 20px 0 10px;
      position: relative;
    }

    a {
      font-weight: 600;
      text-decoration: none;
      font-size: .9rem;
      color: #000;

      &:hover {
        font-weight: 700;
      }
    }
  }

}
.search-bar {
  border: 1px solid #222;
  border-radius: 50px;
  height: 40px;
  width: 300px;
  max-width: 100%;
  position: relative;

  i {
    position: absolute;
    left: 10px;
    top: 50%;
    transform: translateY(-50%);
    color: #4f4f4f;
  }

  input {
    border-radius: 50px;
    padding-left: 35px;
    border: none;
    outline: none;
    width: 100%;
    height: 100%;
    background-color: transparent;
    &::placeholder {
      font-size: .9rem;
    }
  }
}

@keyframes fly-down {
  to {
    transform: translateY(0);
    pointer-events: all;
    opacity: 1;
  }
}

div.nav__items {
  @media screen and (max-width: 992px) {
    flex-direction: column;
    margin: 0;
    width: 100%;
    position: fixed;
    background-color: #FFCC00;
    height: calc(100vh - 60px);
    z-index: 1;
    top: 60px;
    left: 0;
    transform: translateY(-1000px);
    pointer-events: none;
    opacity: 0;
    flex-wrap: nowrap;
    overflow-y: auto;
    padding-top: 20px;

    li {
      margin: 10px 0;
      text-align: center;
    }

    &.active {
      animation: ease .7s fly-down forwards;
    }
  }
}

.hamburger {
  width: 40px;
  background-color: transparent;
  cursor: pointer;
  border: none;
  outline: none;
}

.hamburger span {
  display: block;
  width: 100%;
  box-shadow: 0 2px 10px 0 rgba(0,0,0,0.3);
  border-radius: 3px;
  height: 2px;
  background: #000;
  transition: all .3s;
  position: relative;
}

span + span {
  margin-top: 8px;
}

.hamburger.active span:nth-child(1) {
  animation: ease .7s top forwards;
}

.hamburger.not-active span:nth-child(1) {
  animation: ease .7s top-2 forwards;
}

.hamburger.active span:nth-child(2) {
  animation: ease .7s scaled forwards;
}

.hamburger.not-active span:nth-child(2) {
  animation: ease .7s scaled-2 forwards;
}

.hamburger.active span:nth-child(3) {
  animation: ease .7s bottom forwards;
}

.hamburger.not-active span:nth-child(3) {
  animation: ease .7s bottom-2 forwards;
}

@keyframes top {
  0% {
    top: 0;
    transform: rotate(0);
  }
  50% {
    top: 10px;
    transform: rotate(0);
  }
  100% {
    top: 10px;
    transform: rotate(45deg);
  }
}

@keyframes top-2 {
  0% {
    top: 10px;
    transform: rotate(45deg);
  }
  50% {
    top: 10px;
    transform: rotate(0deg);
  }
  100% {
    top: 0;
    transform: rotate(0deg);
  }
}

@keyframes bottom {
  0% {
    bottom: 0;
    transform: rotate(0);
  }
  50% {
    bottom: 10px;
    transform: rotate(0);
  }
  100% {
    bottom: 10px;
    transform: rotate(135deg);
  }
}

@keyframes bottom-2 {
  0% {
    bottom: 10px;
    transform: rotate(135deg);
  }
  50% {
    bottom: 10px;
    transform: rotate(0);
  }
  100% {
    bottom: 0;
    transform: rotate(0);
  }
}

@keyframes scaled {
  50% {
    transform: scale(0);
  }
  100% {
    transform: scale(0);
  }
}

@keyframes scaled-2 {
  0% {
    transform: scale(0);
  }
  50% {
    transform: scale(0);
  }
  100% {
    transform: scale(1);
  }
}

@keyframes fly-up {
  from {
    transform: translateY(40px);
    opacity: 0;
  }
}

@keyframes fly-right {
  from {
    transform: translateX(-40px);
    opacity: 0;
  }
}

ul.sub-menu {
  background-color: #1D1D1D;
  color: #FFF;
  position: absolute;
  border-radius: 10px;
  animation: ease .5s fly-up;
  li {
    text-align: left;
    padding: 20px;
    border-bottom: 1px solid #FFF;
    &:first-child {
      border-radius: 10px 10px 0 0;
    }

    &:last-child {
      border-radius: 0 0 10px 10px;
      border-bottom: none;
    }

    &:hover {
      background-color: rgba($color: #FFF, $alpha: 0.2);
    }

    a {
      color: #FFF;
      white-space: nowrap;
    }
  }

  @media screen and (max-width: 992px) {
    position: relative;
  }

  &--sub {
    left: 100%;
    top: 0;
    animation: ease .5s fly-right;
    @media screen and (max-width: 992px) {
      display: none !important;
    }
  }
}
</style>
