<template>
  <div class="container">
    <input v-model="movie.title" type="text" placeholder="Movie title" class="form-control">
    <input v-model="movie.year" type="text" placeholder="Movie year" class="form-control">
    <button v-on:click="add(movie)" type="button" class="btn btn-primary">Add</button>
    <div class="container">
      <div class="row">
        <div v-for="(movie, index) in movies" :key="index" class="col">
          <Card :title="movie.title" :text="movie.year" btn="Go to movie"></Card>
          <button v-on:click="remove(index)" type="button" class="btn btn-danger">Remove</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Card from "./components/Card";

export default {
  name: 'App',
  components: {
    Card
  },
  data() {
    return {
      movie: {},
      movies: [
        {id: 1, title: "Terminator", year: "1990"},
        {id: 2, title: "Fast and furious", year: "2001"},
      ]
    }
  },
  methods: {
    add(movie) {
      this.movies.push(movie);
    },
    remove(index) {
      this.movies.splice(index, 1);
    }
  }
}
</script>