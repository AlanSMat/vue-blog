<template>
  <div id="app">
    <Header/>
    <router-view/>
    <add-blog></add-blog>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/layout/Header.vue";
import Footer from "@/components/layout/Footer.vue";
import addBlog from "@/components/addBlog.vue";

export default {
  components: {
    Header,
    Footer,
    "add-blog": addBlog
  }
};
</script>

<style lang="scss">
body {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  margin: 0;
  padding: 0;
}
button {
  padding: 5px 15px;
  color: rgb(97, 89, 89);
  background: #ccc;
  border: 1px solid #333;
  cursor: pointer;
  margin: auto;
  cursor: pointer;
}

button:hover {
  color: #ccc;
  background: #333;
}
</style>
