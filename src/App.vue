<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <router-link to="/" class="navbar-brand">Home</router-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link class="nav-link active" aria-current="page" to="/list">Page List</router-link>
            <!-- <a class="nav-link active" aria-current="page" href="#">Link01</a> -->
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link02</a>
          </li>
        </ul>
        <!-- <form class="d-flex" role="search">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form> -->
      </div>
    </div>
  </nav>
 
  <router-view :dataList="blogData" ></router-view>

  <!-- <TheList :dataList="blogData" /> -->

</template>
<script>
//import TheList from './components/TheList.vue'
import blogData from './assets/blog'

export default {
  name: 'App',
  data() {
    return {
      blogData: blogData
    }
  },
  components: {
    //TheList : TheList,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.navbar-brand {
  margin-left: 360px;
}
</style>
