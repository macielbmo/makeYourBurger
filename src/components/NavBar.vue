<template>
  <nav id="nav">
    <div id="nav-container">
      <router-link to="/" id="logo-url">
        <img :src="logo" :alt="alt" id="logo" />
      </router-link>
      <router-link to="/">Home</router-link>
      <router-link to="/pedidos">Pedidos</router-link>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  props: ["logo", "alt"],
};
</script>

<style scoped>
#nav {
  background-color: #222;
  border-bottom: 4px solid #111;
  padding: 15px 50px;
  display: flex;
}

#nav-container {
  width: 940px;
  margin: 0 auto;
  display: flex;
  align-items: center;
}

#nav-container #logo-url {
  margin: auto;
  margin-left: 0;
}

#logo {
  width: 40px;
  height: 40px;
}

#nav-container a {
  color: #fcba03;
  text-decoration: none;
  margin: 12px;
  transition: 0.5s;
}

#nav-container a:hover {
  color: #fff;
}
</style>
