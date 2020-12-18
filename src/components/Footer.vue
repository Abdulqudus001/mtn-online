<template>
  <footer class="footer">
    <div class="my-container row mx-auto px-0">
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> Personal </a>
        </h4>
        <ul>
          <li>
            <a href="#"> Services </a>
          </li>
          <li>
            <a href="#"> Data </a>
          </li>
          <li>
            <a href="#"> Devices </a>
          </li>
          <li>
            <a href="#"> Getting Started </a>
          </li>
          <li>
            <a href="#"> myMTN App </a>
          </li>
        </ul>
      </div>
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> Business </a>
        </h4>
      </div>
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> Investors </a>
        </h4>
        <ul>
          <li>
            <a href="#"> More in Investors </a>
          </li>
          <li>
            <a href="#"> Shareholders </a>
          </li>
          <li>
            <a href="#"> Financial Reporting </a>
          </li>
          <li>
            <a href="#"> Announcements </a>
          </li>
        </ul>
      </div>
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> Foundation </a>
        </h4>
      </div>
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> Events </a>
        </h4>
      </div>
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> Support </a>
        </h4>
        <ul>
          <li>
            <a href="#"> Help Center </a>
          </li>
          <li>
            <a href="#"> Community </a>
          </li>
        </ul>
      </div>
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> About Us </a>
        </h4>
      </div>
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> Careers </a>
        </h4>
      </div>
      <div class="footer__item col-12 col-md-4 col-lg-2 pl-0">
        <h4>
          <a href="#"> Contact Us </a>
        </h4>
        <ul>
          <li>
            <a href="#"> MTN Supplier </a>
          </li>
        </ul>
      </div>
      <div class="footer__item col-12">
        <div class="row">
          <div class="col-12 col-md-6">
            <div class="icons">
              <a href="#">
                <i class="fab fa-facebook-f"></i>
              </a>
              <a href="#">
                <i class="fab fa-twitter"></i>
              </a>
              <a href="#">
                <i class="fab fa-linkedin-in"></i>
              </a>
              <a href="#">
                <i class="fab fa-youtube"></i>
              </a>
              <a href="#">
                <i class="fab fa-instagram"></i>
              </a>
            </div>
            <p class="copy mt-3">
              &copy; 2020 MTN Nigeria Communications PLC, All rights reserved
            </p>
            <p class="copy">
              <a href="#"> Privacy Policy & Data Protection </a>
            </p>
          </div>
          <div class="col-12 col-md-6">
            <select name="" id="">
              <option
                v-for="country in options"
                :key="country"
                :value="country"
              >
                {{ country }}
              </option>
            </select>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data: () => ({
    options: [
      'Afghanistan',
      'Benin',
      'Botswana',
      'Cameroon',
      'Congo',
      'Ghana',
      'Guinea Bissau',
      'Guinea Conakry',
      'Iran',
      'Ivory Coast',
      'Liberia',
      'Namibia',
      'Nigeria',
      'Rwanda',
      'South Africa',
      'South Sudan',
      'Sudan',
      'Swaziland',
      'Syria',
      'Uganda',
      'Yemen',
      'Zambia',
    ],
  }),
};
</script>

<style lang="scss" scoped>
.footer {
  background-color: #000;
  color: #fff;
  padding: 40px 0;
  text-align: center;

  &__item {
    font-size: 0.9rem;
    h4 {
      font-size: 0.9rem;
      font-weight: 700;
      margin: 20px 0;
    }

    li {
      font-weight: 100;
      margin: 10px 0;
      &:hover {
        opacity: 0.7;
      }
    }

    a {
      text-decoration: none;
      color: #fff;
    }
  }

  .icons {
    width: 300px;
    max-width: 100%;
    display: flex;
    justify-content: space-between;
    font-size: 1.5rem;

    a {
      margin-right: 30px;
      transition: color 0.2s ease-out;
      &:hover {
        color: #ffcc00;
      }
    }
  }

  .copy,
  .copy a {
    font-size: 0.8rem;
    font-weight: 100;
    margin: 0 0 10px;
    color: rgba($color: #fff, $alpha: 0.3);
  }

  select {
    min-height: 40px;
    width: 200px;
    max-width: 100%;
    border-radius: 50px;
    color: #FFF;
    background-color: #000;
    padding: 0 20px;
    border: 2px solid #FFF;
    appearance: none;
    background-image: url('data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4KPHN2ZyB3aWR0aD0iMTJweCIgaGVpZ2h0PSI4cHgiIHZpZXdCb3g9IjAgMCAxMiA4IiB2ZXJzaW9uPSIxLjEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiPgogICAgPCEtLSBHZW5lcmF0b3I6IFNrZXRjaCA1MS4zICg1NzU0NCkgLSBodHRwOi8vd3d3LmJvaGVtaWFuY29kaW5nLmNvbS9za2V0Y2ggLS0+CiAgICA8dGl0bGU+U2hhcGUgQ29weTwvdGl0bGU+CiAgICA8ZGVzYz5DcmVhdGVkIHdpdGggU2tldGNoLjwvZGVzYz4KICAgIDxkZWZzPjwvZGVmcz4KICAgIDxnIGlkPSJQYWdlLTEiIHN0cm9rZT0ibm9uZSIgc3Ryb2tlLXdpZHRoPSIxIiBmaWxsPSJub25lIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiPgogICAgICAgIDxnIGlkPSJTaGFwZS1Db3B5IiBmaWxsPSIjRkZGRkZGIiBmaWxsLXJ1bGU9Im5vbnplcm8iPgogICAgICAgICAgICA8cG9seWdvbiBpZD0icGF0aC0xIiBwb2ludHM9IjEuNDEgMCA2IDQuNTggMTAuNTkgMCAxMiAxLjQxIDYgNy40MSAwIDEuNDEiPjwvcG9seWdvbj4KICAgICAgICA8L2c+CiAgICA8L2c+Cjwvc3ZnPg==');
    background-repeat: no-repeat;
    background-position: 90% 50%;
    outline: none;

    &:active {
      background-color: #FFF;
      color: #000;
    }
  }

  @media screen and (min-width: 992px) {
    // margin-top: 100px;
    // overflow-x: hidden;
    padding: 80px 0;
    text-align: left;
    position: relative;
    &:before {
      box-shadow: 0 0 0 40px #F2F2F2;
      border-radius: 100%;
      position: absolute;
      left: 0;
      right: 0;
      top: 0;
      height: 5px;
      background-color: #F2F2F2;
      content: '';
      transform: rotate(180deg);
    }
  }
}
</style>
