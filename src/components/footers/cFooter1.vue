<template>
  <div id="cFooter1">
    <div class="container row align-items-center" style="margin: auto">
      <div class="row mt-5 rowtop">
        <div class="col">
          <router-link class="navbar-brand" to="/">
            <img src="@/assets/logo.png" width="150" height="150" alt="" />
          </router-link>
        </div>
        <div class="col d-flex align-items-center justify-content-center">
          <div class="row">
            <i class="col-lg-4 lab la-facebook-f"></i>
            <i class="col-lg-4 lab la-linkedin-in"></i>
            <i class="col-lg-4 lab la-twitter"></i>
          </div>
        </div>
      </div>
      <h5 style="font-size: 30px">CONTACT</h5>
      <div class="row mt-3">
        <div class="col-lg-4">
          <h5>CURAÇAO CHAMBER OF COMMERCE & INDUSTRY</h5>
          <ul>
            <li><a>Kaya Junior Salas 1</a></li>
            <li><a>Pietermaai, Curaçao</a></li>
          </ul>
          <ul style="margin-top: 15px">
            <li><a>BUSINESS HOURS</a></li>
            <li><a>Monday - Friday 8:00 - 15:00 non-stop</a></li>
          </ul>
        </div>
        <div class="col-lg-4">
          <h5>TELEPHONE NUMBERS</h5>
          <ul>
            <li><a>(+599-9) 461-1451 (Management)</a></li>
            <li><a>(+599-9) 461-1455 (Registry Affairs)</a></li>
            <li>
              <a
                >(+599-9) 461-3918 (Curaçao Business Information Center /
                Investment Promotion & Business Activities)</a
              >
            </li>
          </ul>
        </div>
        <div class="col-lg-4">
          <h5>E-MAIL</h5>
          <ul>
            <li><a>management@curacao-chamber.cw (Management)</a></li>
            <li><a>registry@curacao-chamber.cw (Registry Affairs)</a></li>
            <li>
              <a
                >businessinfo@curacao-chamber.cw (Curaçao Business Information
                Center / Investment Promotion & Business Activities)</a
              >
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
#cFooter1 {
  background: #073677;
  .container {
    min-height: 500px;

    .rowtop {
      border-bottom: 2px solid rgb(209, 209, 189);
    }
    h5 {
      font-size: 16px;
      color: rgb(209, 209, 189);
    }
    ul {
      list-style: none;
      font-size: 5px;
      li {
        a {
          color: rgba(209, 209, 189, 0.644);
          text-decoration: none;
          font-size: 16px;
        }
      }
    }
    i {
      cursor: pointer;
      color: #073677;
      font-size: 50px;
      background: #e9ecefbd;
      border-radius: 50%;
      width: 50px;
      height: 50px;
      padding: 0;
      margin: 0 10px;
      text-align: center;
      &:hover {
        background: white;
      }
      @media screen and (max-width: 600px) {
        font-size: 30px;
        width: 30px;
        height: 30px;
      }
    }
  }
}
</style>
