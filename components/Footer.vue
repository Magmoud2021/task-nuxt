<template>
  <div>
    <div class="row">
      <div class=" col col-sm-12">
        <p>{{ name }}</p>
        <p>{{ titel }}</p>
        <p>{{ phone }}</p>
      </div>
    </div>

    <footer class="text-center text-white" style="background-color: #caced1">
      <!-- Grid container -->
      <div class="container p-4">
        <!-- Section: Images -->
        <section class="">
          <div class="row">
            <div class="col-lg-2 col-md-12 mb-4 mb-md-0">
              <div
                class="bg-image hover-overlay ripple shadow-1-strong rounded"
                data-ripple-color="light"
              >
                <img
                  src="https://mdbcdn.b-cdn.net/img/new/fluid/city/113.webp"
                  class="w-100"
                />
                <a href="#!">
                  <div
                    class="mask"
                    style="background-color: rgba(251, 251, 251, 0.2)"
                  ></div>
                </a>
              </div>
            </div>
            <div class="col-lg-2 col-md-12 mb-4 mb-md-0">
              <div
                class="bg-image hover-overlay ripple shadow-1-strong rounded"
                data-ripple-color="light"
              >
                <img
                  src="https://mdbcdn.b-cdn.net/img/new/fluid/city/111.webp"
                  class="w-100"
                />
                <a href="#!">
                  <div
                    class="mask"
                    style="background-color: rgba(251, 251, 251, 0.2)"
                  ></div>
                </a>
              </div>
            </div>
            <div class="col-lg-2 col-md-12 mb-4 mb-md-0">
              <div
                class="bg-image hover-overlay ripple shadow-1-strong rounded"
                data-ripple-color="light"
              >
                <img
                  src="https://mdbcdn.b-cdn.net/img/new/fluid/city/112.webp"
                  class="w-100"
                />
                <a href="#!">
                  <div
                    class="mask"
                    style="background-color: rgba(251, 251, 251, 0.2)"
                  ></div>
                </a>
              </div>
            </div>
            <div class="col-lg-2 col-md-12 mb-4 mb-md-0">
              <div
                class="bg-image hover-overlay ripple shadow-1-strong rounded"
                data-ripple-color="light"
              >
                <img
                  src="https://mdbcdn.b-cdn.net/img/new/fluid/city/114.webp"
                  class="w-100"
                />
                <a href="#!">
                  <div
                    class="mask"
                    style="background-color: rgba(251, 251, 251, 0.2)"
                  ></div>
                </a>
              </div>
            </div>
            <div class="col-lg-2 col-md-12 mb-4 mb-md-0">
              <div
                class="bg-image hover-overlay ripple shadow-1-strong rounded"
                data-ripple-color="light"
              >
                <img
                  src="https://mdbcdn.b-cdn.net/img/new/fluid/city/115.webp"
                  class="w-100"
                />
                <a href="#!">
                  <div
                    class="mask"
                    style="background-color: rgba(251, 251, 251, 0.2)"
                  ></div>
                </a>
              </div>
            </div>
            <div class="col-lg-2 col-md-12 mb-4 mb-md-0">
              <div
                class="bg-image hover-overlay ripple shadow-1-strong rounded"
                data-ripple-color="light"
              >
                <img
                  src="https://mdbcdn.b-cdn.net/img/new/fluid/city/116.webp"
                  class="w-100"
                />
                <a href="#!">
                  <div
                    class="mask"
                    style="background-color: rgba(251, 251, 251, 0.2)"
                  ></div>
                </a>
              </div>
            </div>
          </div>
        </section>
        <!-- Section: Images -->
      </div>
      <!-- Grid container -->

      <!-- Copyright -->
      <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2)">
        © 2020 Copyright:
        <a class="text-white" href="https://mdbootstrap.com/"
          >MDBootstrap.com</a
        >
      </div>

      <!-- Copyright -->
    </footer>
  </div>
</template>
<script>
export default {
  name: "Footer",
  data() {},
  props: {
    name: {
      type: String,
    },
    titel: {
      type: String,
    },
    phone: {
      type: Number,
    },
    // onarray: {
    //   type: Array,
    // },
  },
};
</script>
<style scoped>
.foot {
  background-color: gray;
  height: 300px;
}
.col {
  display: flex;
  justify-content: space-around;
  align-items: center;

}
</style>
