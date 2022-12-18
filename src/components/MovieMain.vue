<!-- <template>
  <div>
    <div class="movie-detail">
      <img :src="movieImage" alt="Movie" />
      <p>{{ movie.title }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["movie"],
  computed: {
    movieImage(){
      return require(`../assets/${this.movie.imageName}`)
    }
  }
};
</script>

<style>
.movie-detail img {
  border-radius: 20px;
  width: 230px;
  height: 350px;
}

.movie-detail {
  margin: 7px;
}

.movie-detail p {
  margin-top: 15px;
  font-weight: 1000;
}
</style> -->

<template>
  <div>
    <div class="movie-detail">
      <img :src="movieImage" alt="Movie" />
      <p>{{ movieTitle }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["movie"],
  data() {
    return {
      movieTitle: this.movie.title,
      movieImage: require(`../assets/${this.movie.imageName}`)
    }
  },
};
</script>

<style>
.movie-detail img {
  border-radius: 20px;
  width: 230px;
  height: 350px;
}

.movie-detail {
  margin: 7px;
}

.movie-detail p {
  margin-top: 15px;
  font-weight: 1000;
}
</style>