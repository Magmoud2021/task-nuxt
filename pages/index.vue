<template>
  <div>
    <NavigatinBar />
    <div class="row row-cols-1 row-cols-md-2 g-4 asd">
      <div class="col">
        <div class="card">
          <img
            src="@/assets/imge/pexels-photo-220453.jpeg"
            class="card-img-top"
            alt="..."
          />
          <div class="card-body">
            <h5 class="card-title">{{cardtitel}}</h5>
            <p class="card-text">
              This is a longer card with supporting text below as a natural
              lead-in to additional content. This content is a little bit
              longer.
            </p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img
            src="@/assets/imge/pexels-photo-220453.jpeg"
            class="card-img-top"
            alt="..."
          />
          <div class="card-body">
            <h5 class="card-title">{{cardtitel}}</h5>
            <p class="card-text">
              This is a longer card with supporting text below as a natural
              lead-in to additional content. This content is a little bit
              longer.
            </p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img
            src="@/assets/imge/pexels-photo-220453.jpeg"
            class="card-img-top"
            alt="..."
          />
          <div class="card-body">
            <h5 class="card-title">{{cardtitel}}</h5>
            <p class="card-text">
              This is a longer card with supporting text below as a natural
              lead-in to additional content.
            </p>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img
            src="@/assets/imge/pexels-photo-220453.jpeg"
            class="card-img-top"
            alt="..."
          />
          <div class="card-body">
            <h5 class="card-title">{{cardtitel}}</h5>
            <p class="card-text">
              This is a longer card with supporting text below as a natural
              lead-in to additional content. This content is a little bit
              longer.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="splide">
      <div class="splide__track">
        <ul class="splide__list">
          <li class="splide__slide">
            <div class="splide__slide__container">
              <img src="@/assets/imge/logo.png" />
            </div>
            Lorem Ipsum Dolor Sit Amet
          </li>
          <li class="splide__slide">
            <div class="splide__slide__container">
              <img src="@/assets/imge/logo.png" />
            </div>
            Lorem Ipsum Dolor Sit Amet
          </li>
        </ul>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import axios from "axios";
import splide from "@splidejs/splide";

export default {
  components: {
    axios,
   splide,
  },
  name: "IndexPage",
  data(){
    return{
      cardtitel:"your profile",
    }
  }
};
</script>
<style scoped>
.asd {

  margin-top: 50px;
  padding-left: 20px;
  padding-right: 20px;
}
img{
  border-radius:5px;
}

</style>
