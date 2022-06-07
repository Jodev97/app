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
  h2 {
    text-transform: uppercase;
  }
}
</style>
