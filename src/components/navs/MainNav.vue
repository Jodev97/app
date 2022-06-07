<template>
  <nav
    class="navbar navbar-expand-lg navbar-light bg-light justify-content-between"
  >
    <div class="container">
      <router-link class="navbar-brand" to="/">
        <img src="@/assets/logo.png" width="30" height="30" alt="" />
      </router-link>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbar"
        aria-controls="navbar"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbar">
        <form
          class="form-inline my-2 my-lg-0 d-flex justify-content-between row"
        >
          <input
            class="form-control mr-sm-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">
            Search
          </button>
        </form>
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <router-link class="nav-link" to="/">HOME</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">ABOUT</router-link>
          </li>

          <li class="nav-item">
            <router-link class="nav-link" to="/curacao"
              >CURAÇAO AT A GLANCE</router-link
            >
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/services">SERVICES</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/business"
              >BUSINESS IN CURAÇAO</router-link
            >
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/news"
              >NEWS & ACTIVITIES</router-link
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss">
#navbar {
  flex-direction: column;
}
</style>
