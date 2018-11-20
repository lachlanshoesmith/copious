<template>
  <div id="app">
    <nav>
      <header>copious</header>
    </nav>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'copious',
};
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: 'Cera Round Basic';
}
body {
  background: linear-gradient(45deg, hsl(155, 65%, 90%), hsl(155, 53%, 88%));
  background-size: cover;
}
nav {
  background: hsl(154, 96%, 90%);
  padding: 10px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
}
header {
  color: hsl(130, 23%, 25%);
  font-weight: bold;
  font-size: 18px;
}
</style>
