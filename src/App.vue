<template>
  <div class="container">
    <Header />
    <FloatingNav />
    <router-view />
  </div>
</template>

<script>
import FloatingNav from "./components/FloatingNav";
import Header from "./components/Header";

export default {
  name: "App",
  components: {
    FloatingNav,
    Header,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;1,100;1,200&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}

.container {
  max-width: 1200px;
  padding: 0 14px;
  margin: 0 auto;
}
</style>
