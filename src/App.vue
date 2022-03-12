<template>
  <div id='app' class = 'page'>
      <div class='section title'>
          Talia Bird Photography
      </div>
      <router-link class='section menu-item link-item'
            to='/'>
          Home
        </router-link>
      <router-link class='section menu-item link-item'
            to='/portfolio'>
          Portfolio
        </router-link>
      <router-link class='section menu-item link-item'
            to='/about'>About
      </router-link>
    <router-view/>

    <a class='section footer link-item' href='https://github.com/BYUCS260/lab-1-photography-website-taliaebird'
    target='_blank'>Git Hub
    </a>

  </div>

</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: snow;
  border: 0px;
}
.page {
  display: flex;
  flex-wrap: wrap;
  background-color: snow;
  justify-content: center;
}
#app {
  background-color: snow;
}
.section {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  flex-direction: column;
  text-align: center;
}

.title {
  background-color: black;
  color: snow;
  width: 40%;
  height: 100px;
}
.menu-item {
  display: flex;
  background-color: black;
  color: snow;
  width: 20%;
  height: 100px;
}

.footer {
  background-color: black;
  height: 75px;
  text-align: left;
  color: snow;
}
.link-item:hover,
.link-item:visited:hover {
  background-color: #989898;
}
a {
  text-decoration: none;
  color: snow;
}
</style>
