<template>
  <div class="container mt-5">
    <h2 class="mb-2">Events</h2>
    <h6>Lorem ipsum, dolor sit.</h6>
    <div class="row">
      <div class="card" style="width: 18rem">
        <img src="@/assets/bg_3.jpg" class="card-img-top" />
        <div class="card-body">
          <h5 class="card-title">Card title</h5>
          <h6 class="card-text">Some quick example text to</h6>
        </div>
      </div>
    </div>

    <div class="row">
      <div class="card" style="width: 18rem; margin-top: 30px">
        <div class="card-body">
          <h5 style="font-weight: bold">
            <i class="las la-angle-right" style="color: red"></i>Stay informed?
          </h5>
          <h6 class="card-text">
            Want to stay informed on our latest news/events? Enter your e-mail
            address here.
          </h6>
          <form action="" class="form-control stacked">
            <input
              type="text"
              name="subscribe-box"
              placeholder="Email"
              class="input-text"
            />
            <button class="btn btn-primary" style="margin-top: 15px">
              Suscribirse
            </button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.card-title {
  font-weight: bold;
  font-size: 15px;
  font-weight: 500;
  margin: 0 0 16px 0;
}
.card-text {
  font-size: 15px;
  font-weight: 500;
  margin: 0 0 16px 0;
}
.form-control {
  margin-left: -10px;
  width: max-content;
  border-radius: 1rem;
}
.btn {
  cursor: pointer;
  border: 1px solid transparent;
  border-radius: 4px;
  margin: 0;
  padding: 10px 20px;
  text-decoration: none;
  text-align: center;
  font-size: 16px;
  background: transparent;
  color: #303030;
  white-space: nowrap;
  vertical-align: middle;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  background: #fff;
}
.btn-primary,
.btn-primary-border,
.primary {
  background: #3498db;
  color: white;
}
.form-control {
  border: 1px solid #e0e0e0;
  padding: 10px 10px;
  text-decoration: none;
  text-align: left;
  font-size: 16px;
  background: #fff;
  color: #303030;
  border-radius: 4px;
  display: inline-flex;
}
.form-control.stacked {
  display: flex;
  -webkit-box-flex: 0;
  -webkit-flex: 0 0 auto;
  -ms-flex: 0 0 auto;
  flex: 0 0 auto;
  -webkit-box-orient: vertical;
  -webkit-flex-direction: column;
  -ms-flex-direction: column;
  flex-direction: column;
}
input.input-text {
  border-radius: 4px;
  border: 1px solid #ccc;
  background: #f9f9f9;
  color: #303030;
  padding: 10px;
  text-decoration: none;
  text-align: left;
  font-size: 1em;
}
</style>
