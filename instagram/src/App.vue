<template>
  <div id="app">
    <nav id="nav" variant="faded" type="light">
      <div class="nav_2">
        <div class="nav_3"> 
          <div class="main-logo-1">
            <a href="#"><img class="main-logo" :src="require('@/assets/insta_logo.png')"></a>
          </div>
          <div class="logos-1">
            <div class="logos-2">
              <router-link to="/home"><b-icon icon="house" scale="1.5"></b-icon></router-link>
              <router-link to="/"><img class="logo" :src="require('@/assets/paper_plane_icon.png')"></router-link>
              <router-link to="/"><b-icon icon="plus-square" scale="1.5"></b-icon></router-link>
              <router-link to="/"><b-icon icon="compass" scale="1.5"></b-icon></router-link>
              <router-link to="/"><b-icon icon="heart" scale="1.5"></b-icon></router-link>

              <router-link to="/"><b-icon icon="person-circle" scale="1.5"></b-icon></router-link>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <div class="home">
      <router-link to="/"></router-link>
    </div>
    <router-view/>
  </div>
</template>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #262626;
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
  position: fixed;
  z-index: 999;
}

#nav a {
  font-weight: bold;
  color: #262626;
}

#nav a.router-link-exact-active {
}
.main-logo {
  width: 103px;
  height: 29px;
  object-fit: contain;
}
.nav_2 {
  border-bottom: 1px solid rgb(218, 218, 218);
  height: 54px;
  position: fixed;
  top: 0;
  width: 100%;
  background-color: #ffffff;
  position: fixed;
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
.logos-2 > * {
  margin-left: 20px;
}

</style>
