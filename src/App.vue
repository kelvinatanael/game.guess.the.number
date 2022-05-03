<template>
  <div id="app">
    <main>
      <router-view/>
    </main>
  </div>
</template>

<style lang="scss">

@import './assets/scss/generic/mixins.scss';
@import './assets/scss/generic/fonts.scss';
@import './assets/scss/generic/utilities.scss';

:root {
  --white: #fff;
  --black-light: #262A34;
  --black: #000;
  --orange: #EF6C00;
  --orange-2: #FF6600;
  --gray: #DDDDDD;
  --gray-2: #CFCFCF;
  --gray-3: #F5F5F5;
  --gray-4: #EEEEEE;
  --green: #32BF00;
  --red: #CC3300;
}
html,
body {
  margin: 0;
  width: 100%;
  min-height: 100vh;
  color: #687188;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  min-height: 100vh;
}
main {
  min-height: 100vh;
}
a {
  text-decoration: none !important;
}
button {
  outline: none !important;
}
</style>
