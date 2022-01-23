<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#"
          ><img src="@/assets/imge/logo.png"
        /></a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavAltMarkup"
          aria-controls="navbarNavAltMarkup"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
          <div class="navbar-nav naa">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
            <a class="nav-link" href="#">Features</a>
            <a class="nav-link" href="#">Pricing</a>
            <a class="nav-link disabled">Disabled</a>
          </div>
        </div>
      </div>
    </nav>
    <div>
      <div class="header">
        <div class="text">
          <h1>{{ name }}<span>salah</span></h1>
          <p>{{ titel }}</p>
        </div>
        <div class="imge">
          <img src="@/assets/imge/pexels-photo-220453.jpeg" />
        </div>
      </div>
    </div>
    <div class="asdd">
      <h3  v-for="album in albums" :key="album">{{ album.title }}</h3>
    </div>

<button  @click="fetchbooks()" type="button" class="btn btn-danger" data-mdb-ripple-color="dark">books</button>

    <!-- <div class="posts">
      <div class="post-card" v-for="book in books" :key="book.id">
        <div class="post-card-body">
          <h3>{{ book.name }}</h3>
          <p>{{ book.id }}</p>
        </div>
      </div>
    </div> -->
  </div>
</template>
<script>
import axios from "@nuxtjs/axios";
export default {
  name: "NavigatinBar",
  components: {
    axios,
  },
  data() {
    return {
      name: "Mahmoud ",
      titel:
        "In this lesson, we're exploring where to put your navbar and other parts",
      albums: {
        userId: "",
        id: "",
        title: "",
      },
    };
  },
  methods: {
    async fetchbooks() {
      const albums = await this.$axios.$get(
        "https://jsonplaceholder.typicode.com/albums/"
      );
      this.albums = albums;
      // console.log("dsfsdfds", books);
    },
  },
  // mounted(){
  //   this.$axios.get('https://vuango-books-api.herokuapp.com/books/').then((res) =>{
  //     this.books=res.data
  //   })
  // }
  // asyncData({ $axios }) {
  //   const books =  $axios.get(
  //       "https://vuango-books-api.herokuapp.com/books/"
  //   )
  //   return{
  //     books:  books

  //   }
  // }

  // async asyncData({ $axios }) {
  //   const books = await $axios.$get(
  //     "https://vuango-books-api.herokuapp.com/books/"
  //   );
  //   return { books };
  // },

  // asyncdata({$axios}) {
  //   return $axios
  //     .$get("https://vuango-books-api.herokuapp.com/books/")
  //     .then((res) => {
  //       return{
  //       books:res
  //       }
  //     });
  // },
};
</script>
<style scoped>
img {
  width: 50px;
}
@media (max-width: 768px){
img {
  display: none;
}
.text h1{
  text-align: center;
}
.text p{
  text-align: center;
}
}
.header {
  background-image: linear-gradient(rgba(255, 0, 0, 0), rgba(255, 0, 0, 1)),
    url(@/assets/imge/shanghai.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  width: 100%;
  height: 500px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.imge img {
  width: 200px;
  border-radius: 50%;
}
h1 {
  font-size: 50px;
  font-family: Arial, Helvetica, sans-serif;
  text-transform: capitalize;

  color: rgb(20, 9, 0);
}
p {
  color: rgb(255, 191, 180);
  font-size: 15px;
  font-family: sans-serif;
  letter-spacing: 5px;
}
span {
  color: orange;
  font-size: 40px;
}
.asdd {
  display: flex;
  justify-content: space-around;
  align-items: center;
  display: inline-block;
}
h3 {
  width: 100%;
  margin: auto;
  color: red;
}
  .naa a{
  margin-right: 50px;
}
</style>
