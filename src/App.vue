<template>
  <div id="app">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<style> 
#app {
  font-family: 'Noto Sans KR', sans-serif;
}

ul {
  padding-left: 0;
  list-style: none;
}
</style>
