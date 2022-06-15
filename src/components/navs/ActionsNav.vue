<template>
  <div class="container">
    <h3>QUICK LINKS</h3>
    <div class="row">
      <ul class="nav justify-content-center">
        <li class="nav-item">
          <router-link class="nav-link active" to="/registry"
            ><i class="lab la-wpforms ico"></i> Registry forms
            <i class="las la-angle-right"></i
          ></router-link>
        </li>
        <li class="nav-item">
          <routerLink class="nav-link" to="/startingUp"
            ><i class="las la-user-tie ico"></i> Starting a business
            <i class="las la-angle-right"></i
          ></routerLink>
        </li>
        <li class="nav-item">
          <routerLink class="nav-link" to="/proposals-to-dissolve"
            ><i class="las la-users-cog ico"></i> Proposals to Dissolve
            <i class="las la-angle-right"></i
          ></routerLink>
        </li>
        <li class="nav-item">
          <routerLink class="nav-link" to="/contact-organisations"
            ><i class="las la-sitemap ico"></i> Contact organisations
            <i class="las la-angle-right"></i
          ></routerLink>
        </li>
      </ul>
    </div>

    <div class="row">
      <ul class="nav justify-content-center">
        <li class="nav-item">
          <routerLink class="nav-link active" to="/tariffs"
            ><i class="las la-user-tag ico"></i> Tariffs
            <i class="las la-angle-right"></i
          ></routerLink>
        </li>
        <li class="nav-item">
          <routerLink class="nav-link" to="/business-opportunities"
            ><i class="las la-business-time ico"></i> Business opportunities
            <i class="las la-angle-right"></i
          ></routerLink>
        </li>
        <li class="nav-item">
          <routerLink class="nav-link" to="/business-Magazine"
            ><i class="las la-newspaper ico"></i> Curacao Business Magazine
            <i class="las la-angle-right"></i
          ></routerLink>
        </li>
        <li class="nav-item">
          <routerLink class="nav-link" to="/contact"
            ><i class="lar la-id-badge ico"></i> Contact Chamber
            <i class="las la-angle-right"></i
          ></routerLink>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.nav {
  --bs-nav-link-color: #000000;
}
.ico {
  font-size: 40px;
}
</style>
