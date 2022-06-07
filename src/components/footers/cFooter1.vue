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
            <i class="col lab la-facebook-f"></i>
            <i class="col lab la-linkedin-in"></i>
            <i class="col lab la-twitter"></i>
          </div>
        </div>
      </div>
      <div class="row mt-3">
        <div class="col-lg-3">
          <h5>Menu 1</h5>
          <ul>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
          </ul>
        </div>
        <div class="col-lg-3">
          <h5>Menu 2</h5>
          <ul>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
          </ul>
        </div>
        <div class="col-lg-3">
          <h5>Menu 3</h5>
          <ul>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
          </ul>
        </div>
        <div class="col-lg-3">
          <h5>Menu 4</h5>
          <ul>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
            <li><a href="#">link1</a></li>
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
    height: 400px;

    .rowtop {
      border-bottom: 2px solid rgb(209, 209, 189);
    }
    h5 {
      color: rgb(209, 209, 189);
    }
    ul {
      list-style: none;
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
    }
  }
}
</style>
