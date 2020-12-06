<template>
  <div class="col mt-5">
      <div class="row mt-md-5 mt-sm-5 mt-xs-5">
        <div class="col-lg-6 col-xs-12" v-for="(movie, index) of movies" :key="index">
          <div
            class="d-flex justify-content-center align-items-center">
            <div class="p-3">
                <img :src="movie.urlToImage" width="960px" height="960px" alt="imagen noticia" class="img-fluid">
            </div>

            <div class="p-4">
                <h4 class=" font-weight-bold "> {{movie.title}}</h4>
                <hr color="#ccd1d1" size="3" />
              <p class="text-secondary  text-justify ">  
                {{movie.description}}
              </p>
              <h6 class="small font-italic ">{{movie.publishedAt}} </h6>
            </div>
          </div>
          <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
            <a :href="movie.url" target="_black" class="btn btn-danger">Mas</a>
          </div>
          <hr color="#ccd1d1" size=3>
        </div>
      </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "sectionapi",
  data() {
    return {
      movies: null,
    };
  },
  mounted() {
    axios
      .get(
        "http://newsapi.org/v2/top-headlines?country=co&category=science&apiKey=3366e11beeec47df8edad6be97536fa1"
      )
      .then((response) => {
        this.movies = response.data.articles.slice(0, 4);
      });
  },
};
</script>

<style lang="stylus" scoped></style>