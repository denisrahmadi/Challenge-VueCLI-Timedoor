<!-- <template>
  <div>
    <app-header></app-header>
    <main>
      <div class="container">
        <div class="title">
          <h1>NOW SHOWING IN CINEMAS</h1>
        </div>
        <div class="movies">
          <app-movie 
              v-for="movie in movies" :key="movie.id" 
              :movie="movie"
          ></app-movie>
        </div>
      </div>
    </main>
    <app-footer></app-footer>
  </div>
</template>

<script>
import HeaderMain from "./components/HeaderMain.vue";
import FooterMain from "./components/FooterMain.vue";
import MovieMain from "./components/MovieMain.vue";

export default {
  data() {
    return {
      movies: [
        { id: 1, title: "INANG", imageName: "movie1.jpg" },
        { id: 2, title: "KALIAN PANTAS MATI", imageName: "movie2.jpg" },
        { id: 3, title: "HALOWEEN ENDS", imageName: "movie3.jpg" },
        { id: 4, title: "PAMALI", imageName: "movie4.jpg" },
      ],
    }
  },
  components: {
    "app-header": HeaderMain,
    "app-footer": FooterMain,
    "app-movie": MovieMain,
  },
};
</script>

<style>
body {
  margin: 0px;
  font-family: "Roboto", sans-serif;
}

a {
  text-decoration: none;
  color: black;
}

header {
  position: sticky;
  top: 0px;
  background-color: white;
}

.container {
  margin-left: 200px;
  margin-right: 200px;
}

/* Header */

/* Now Showing */
.movies {
  display: flex;
  justify-content: center;
}

.title h1 {
  font-size: 25px;
}
/* Footer */
</style> -->

<template>
  <div>
    <app-header></app-header>
    <main>
      <div class="container">
        <div class="title">
          <h1>NOW SHOWING IN CINEMAS</h1>
        </div>
        <div class="movies">
          <app-movie v-for="data in dataMovie" :key="data.id" :movie="data"></app-movie>
        </div>
      </div>
    </main>
    <app-footer></app-footer>
  </div>
</template>

<script>
import HeaderMain from "./components/HeaderMain.vue";
import FooterMain from "./components/FooterMain.vue";
import MovieMain from "./components/MovieMain.vue";

export default {
  data() {
    return {
      dataMovie: [
        { id: 1, title: "INANG", imageName: "movie1.jpg" },
        { id: 2, title: "KALIAN PANTAS MATI", imageName: "movie2.jpg" },
        { id: 3, title: "HALOWEEN ENDS", imageName: "movie3.jpg" },
        { id: 4, title: "PAMALI", imageName: "movie4.jpg" },
      ],
    };
  },
  components: {
    "app-header": HeaderMain,
    "app-footer": FooterMain,
    "app-movie": MovieMain,
  },
};
</script>

<style>
body {
  margin: 0px;
  font-family: "Roboto", sans-serif;
}

a {
  text-decoration: none;
  color: black;
}

header {
  position: sticky;
  top: 0px;
  background-color: white;
}

.container {
  margin-left: 200px;
  margin-right: 200px;
}

/* Header */

/* Now Showing */
.movies {
  display: flex;
  justify-content: center;
}

.title h1 {
  font-size: 25px;
}
/* Footer */
</style>
