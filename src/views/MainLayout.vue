<template>
  <div class="container bg-ligth">
    <div class="row">
      <div class="col-lg-9 container">
        <slot name="content"></slot>
      </div>
      <div class="col-lg-3 container">
        <slot name="sidebarRigth"></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
