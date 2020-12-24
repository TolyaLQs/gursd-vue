<template>
  <div class="topnav-content">
    <div class="topnav">
      <div class="logo">
        <router-link to="/">Home</router-link>
      </div>
      <div class="topnav-cat-abo">
      <div class="catalog">
        <router-link to="/catalog">Catalog</router-link>
      </div>
      <div class="about">
        <router-link to="/about">About</router-link>
      </div>
      </div>
      <div class="profile">
        <router-link to="/profile">Profile</router-link>
      </div>
    </div>
    <router-view/>
  </div>

</template>

<script>
export default {
  name: "TopNav"
}
</script>


<style scoped>
a{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  text-decoration: none;
  font-size: 25px;
}

a:hover{
  color: darkgrey;
}

.topnav {
  width: 100%;
  height: 50px;
  background-color: black;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.topnav-cat-abo{
  width: 200px;
  display: flex;
  justify-content: space-between;
}

</style>