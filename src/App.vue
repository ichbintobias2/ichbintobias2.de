<template>
  <nav>
    <img src="@/assets/banner.png">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view />
</template>

<style scoped>
nav {
  text-align: center;
  padding: 30px;
}
</style>
