<template>
  <h2>
    Select a <br />
    location for Holiday
  </h2>
  <SearchBar />
  <Categories :categories="categories" />
  <Card />
</template>

<script>
import SearchBar from "../components/SearchBar";
import Categories from "../components/Categories.vue";
import Card from "../components/Card";

export default {
  name: "Home",
  components: {
    SearchBar,
    Categories,
    Card,
  },
  data() {
    return {
      categories: [
        "Christmas",
        "Honeymoon",
        "Tourism",
        "Family",
        "Easter",
        "New Year",
      ],
      locations: [],
    };
  },
};
</script>

<style scoped>
h2 {
  font-style: normal;
  font-weight: 500;
  font-size: 30px;
  line-height: 38px;
  color: #141414;
  margin-top: 40px;
}
</style>
