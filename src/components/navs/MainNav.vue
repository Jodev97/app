<template>
  <nav
    class="navbar navbar-expand-lg navbar-light bg-light justify-content-between"
  >
    <div class="container">
      <router-link class="navbar-brand" to="/">
        <img src="@/assets/logo.png" width="70" height="70" alt="" />
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
        <div class="wrap row mb-2">
          <div class="search">
            <input
              type="text"
              class="searchTerm"
              placeholder="What are you looking for?"
            />
            <button type="submit" class="searchButton">
              <i class="fa fa-search"></i>
            </button>
          </div>
        </div>
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
  li {
    transition: 0.7s ease;
    &:hover {
      background: #073677;
      a {
        color: white;
      }
    }
  }
  .search {
    width: 100%;
    position: relative;
    display: flex;
  }

  .searchTerm {
    width: 100%;
    border: 3px solid #073677;
    border-right: none;
    padding: 5px;
    border-radius: 5px 0 0 5px;
    outline: none;
    color: #9dbfaf;
  }

  .searchTerm:focus {
    color: #073677;
  }

  .searchButton {
    width: 40px;
    border: 1px solid #073677;
    background: #073677;
    text-align: center;
    color: #fff;
    border-radius: 0 5px 5px 0;
    cursor: pointer;
    font-size: 20px;
  }

  /*Resize the wrap to see the search bar change!*/
  .wrap {
    position: relative;
    transform: translate(100%, 0);
  }
}
</style>
