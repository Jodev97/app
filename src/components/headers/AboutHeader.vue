<template>
  <div id="aboutHeader" class="container position-absolute">
    <h2 class="row bg-light w-25">{{ $route.name }}</h2>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
#aboutHeader {
  bottom: 0;
  right: 4em;
  @media screen and (max-width: 600px) {
    right: -1em;
    h2 {
      width: 100% !important;
      font-size: 32px;
    }
  }
  h2 {
    text-transform: uppercase;
  }
}
</style>
