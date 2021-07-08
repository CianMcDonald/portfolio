<template>
  <div id="nav">
    <h2> Cian McDonald </h2>
    <div class="router">
      <router-link to="/">Home</router-link> 
      <router-link to="/about">About</router-link>
    </div>
  </div>
  <router-view/>
</template>

<style>
body {
  padding: 0;
  margin: 0;
  font-family: 'Roboto', sans-serif;
}
h2 {
  margin: 0
}
#nav {
  display: flex;
  justify-content: space-between;
  padding: 30px;
  background-color: #363537;
  color: #F7EBE8;
  align-items: flex-start;
}
#router{
  margin: 0;
  display: flex;
  justify-content: space-between;
}


#nav a {
  font-weight: bold;
  text-decoration: None;
  padding: 0 10px;
  color: #F7EBE8;
}
#nav a:hover {
  color: white;
}
#nav a.router-link-exact-active {
  font-size: 110%;
}
</style>
