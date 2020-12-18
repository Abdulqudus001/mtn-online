<template>
  <div>
    <Nav />
    <main>
      <section class="hero row align-items-center mx-0">
        <a href="#">
          <i class="fa fa-angle-left"></i>
          Back
        </a>
        <div class="my-container row px-0">
          <div class="col-12 col-md-6 px-0">
            <h1 class="hero__title">Contact</h1>
            <h2 class="hero__subtitle">MTN Suppliers</h2>
          </div>
        </div>
        <svg
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          x="0px"
          y="0px"
          height="25px"
          viewBox="0 0 1366 25"
          fill="#FFF"
          xml:space="preserve"
          preserveAspectRatio="none"
          class="mtn-curve__concave mtn-curve__curve-desktop"
        >
          <path
            d="M683.1,23.9C386.6,23.9,129.2,14.1,0,0v25h1366V0C1236.7,14.1,979.4,23.9,683.1,23.9z"
            class="mtn-svg-fill--white"
            style="z-index: 2"
          ></path>
        </svg>
      </section>
      <section class="existing">
        <div class="my-container px-0">
          <h2 class="existing__title">Existing MTN supplier</h2>
          <p>
            MTN has a responsibility to ensure that our business practices are
            conducted according to local and international laws, and adhere to the
            highest levels of ethical and moral conduct.
          </p>
          <p>
            We embrace this across all parts of our business, and we expect the
            same from our suppliers. The Supplier Code of Conduct sets out our
            approach to ethical and sustainable business practices and aims for
            the highest ethical conduct. It outlines our commitment to respect and
            promote human rights and fair workplace practices, including equal
            opportunities, environmentally sustainable business activities, and a
            zero-tolerance policy to bribery and corruption.
          </p>
          <p>
            MTN expects its suppliers to embrace this commitment to integrity by
            complying with and training its employees and subcontractors on the
            Supplier Code of Conduct.
          </p>
          <p>
            By working together, we can make the customer’s lives a whole lot
            brighter.
          </p>
          <div class="existing__cards row">
            <div class="col-12 col-md-6">
              <div class="card">
                <div>
                  Supplier Privacy Notice
                  <span class="card__size"> (2 MB-PDF)</span>
                </div>
                <div class="card__icon">
                  <i class="fa fa-download"></i>
                </div>
              </div>
            </div>

            <div class="col-12 col-md-6">
              <div class="card">
                <div>
                  Code of Conduct
                  <span class="card__size"> (556 KB-PDF)</span>
                </div>
                <div class="card__icon">
                  <i class="fa fa-download"></i>
                </div>
              </div>
            </div>
          </div>
        </div>
        <svg
          version="1.1"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          x="0px"
          y="0px"
          height="25px"
          viewBox="0 0 1366 25"
          fill="#F2F2F2"
          xml:space="preserve"
          preserveAspectRatio="none"
          class="mtn-curve__concave mtn-curve__curve-desktop"
        >
          <path
            d="M683.1,23.9C386.6,23.9,129.2,14.1,0,0v25h1366V0C1236.7,14.1,979.4,23.9,683.1,23.9z"
            class="mtn-svg-fill--white"
            style="z-index: 2"
          ></path>
        </svg>
      </section>
      <section class="supplier">
        <div class="my-container px-0">
          <h2 class="supplier__title">Become an MTN supplier</h2>
          <p>
            If you believe you can join MTN’s vision to make our customers lives a whole lot brighter, then click on apply below to fill in the registration form.
          </p>
          <div class="supplier__cards row">
            <div class="col-12 col-md-6">
              <div class="card">
                <div>
                  Supplier Privacy Notice
                  <span class="card__size"> (2 MB-PDF)</span>
                </div>
                <div class="card__icon">
                  <i class="fa fa-download"></i>
                </div>
              </div>
            </div>

            <div class="col-12 col-md-6">
              <div class="card">
                <div>
                  Code of Conduct
                  <span class="card__size"> (556 KB-PDF)</span>
                </div>
                <div class="card__icon">
                  <i class="fa fa-download"></i>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>
    <Footer />
  </div>
</template>

<script>
import Nav from '@/components/Nav.vue';
import Footer from '@/components/Footer.vue';

export default {
  components: {
    Nav,
    Footer,
  },
};
</script>

<style lang="scss" scoped>
.hero {
  background: linear-gradient(
      rgba($color: #000, $alpha: 0.3),
      rgba($color: #000, $alpha: 0.3)
    ),
    url('../assets/hero.jpg') no-repeat;
  background-size: cover;
  min-height: 550px;
  position: relative;
  color: #fff;

  a {
    background-color: #ffcc00;
    color: #000;
    display: block;
    border-radius: 50px;
    width: 100px;
    padding: 10px 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-style: italic;
    position: absolute;
    top: 20px;
    left: 20px;
    font-size: 0.9rem;
    font-weight: 600;
  }

  svg {
    position: absolute;
    width: 100%;
    bottom: 0;
    @media screen and (max-width: 992px) {
      display: none;
    }
  }

  &__title {
    font-size: 1.5rem;

    @media screen and (min-width: 992px) {
      font-size: 1.8rem;
    }
  }

  &__subtitle {
    font-size: 3rem;
    font-weight: 600;

    @media screen and (min-width: 992px) {
      font-size: 4rem;
    }
  }
}

.existing,
.supplier {
  position: relative;
  padding: 80px 0 40px;

  svg {
    position: absolute;
    width: 100%;
    bottom: 0;
    @media screen and (max-width: 992px) {
      display: none;
    }
  }

  &__title {
    font-weight: 600;
    margin-bottom: 20px;
  }

  p {
    font-weight: 100;
  }

  @media screen and (min-width: 992px) {
    padding: 120px 0 40px;
  }

  .card {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 30px 20px;
    align-items: center;
    font-weight: 600;
    border-radius: 20px;
    transition: box-shadow .3s ease;
    margin-top: 10px;
    margin-bottom: 10px;

    &__icon {
      background-color: #ffcc00;
      border-radius: 50%;
      width: 50px;
      height: 50px;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    &__size {
      display: block;
      font-weight: 400;
      font-size: 0.8rem;
    }

    &:hover {
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
    }
  }
}

.existing {
  @media screen and (min-width: 992px) {
    padding-bottom: 120px;
  }
}

.supplier {
  background-color: #F2F2F2;
  @media screen and (min-width: 992px) {
    padding-bottom: 120px;
  }
}
</style>
