<template>
  <div id="app">
    <nav id="nav" variant="faded" type="light">
      <div class="nav_2">
        <div class="nav_3"> 
          <div class="main-logo-1">
            <img class="main-logo" src="https://www.instagram.com/static/images/web/mobile_nav_type_logo-2x.png/1b47f9d0e595.png" alt="Kitten">
          </div>
          <div class="logos-1">
            <div class="logos-2">
              <router-link to="/"><img class="logo" src="https://cdn-icons-png.flaticon.com/512/2919/2919516.png" alt=""></router-link>
              <router-link to="/"><img class="logo" src="https://cdn-icons.flaticon.com/png/512/880/premium/880557.png?token=exp=1636883505~hmac=beac2f34878af75e3e540b236caaee9d" alt=""></router-link>
              <router-link to="/"><img class="logo" src="https://cdn-icons-png.flaticon.com/512/875/875068.png" alt=""></router-link>
              <router-link to="/"><img class="logo" src="https://cdn-icons-png.flaticon.com/512/2948/2948031.png" alt=""></router-link>
              <router-link to="/"><img class="logo" src="https://cdn-icons-png.flaticon.com/512/812/812327.png" alt=""></router-link>
              <router-link to="/"><img class="logo" src="https://cdn-icons.flaticon.com/png/512/3024/premium/3024605.png?token=exp=1636888433~hmac=eaf432b5d65a01c12c4949dd1402b97f" alt=""></router-link>

            </div>
          </div>
        </div>
      </div>
    </nav>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  order: 0;
  padding: 0;
  align-items: stretch;
  border: 0 solid #000;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  flex-shrink: 0;
  margin: 0;
  position: relative;
  vertical-align: baseline;
  
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.main-logo {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
}
.nav_2 {
  border-bottom: 1px solid rgb(218, 218, 218);
  height: 54px;
  position: fixed;
  top: 0;
  width: 100%;
}
.nav_3 {
  height: 54px;
  align-items: center;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  padding: 0 20px;
  transition: height .2s ease-in-out;
}
.main-logo-1 {
  margin-top: 7px;
  transition: opacity .1s ease-out;
  justify-content: flex-start;
  align-items: stretch;
}
.logo {
  font-size: 50%;
  color: white;
  display: block;
  position: relative;
  height: 22px;
  width: 22px;
  overflow: hidden;
  cursor: pointer;
  white-space: nowrap;
  margin-left: 20px;
}
.logos-1 {
  display: flex;
  flex-direction: row-reverse;
  box-sizing: border-box;
  flex-shrink: 0;
  margin: 0;
  padding: 0;
  position: relative;
  width: 80%;
  height: 22px;
}
.logos-2 {
  display: flex;
  padding-left: 0;
  flex-direction: row;
  align-items: center;
}
</style>
