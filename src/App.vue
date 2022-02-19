<template>
  <div id="app">
    <div id="nav">
       <b-navbar  type="dark">
    <b-navbar-brand href="#"><img height="30" width="120" src="@/assets/icons/header-logo.png" />
      </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="/">Home</b-nav-item>
        <b-nav-item href="#">Events</b-nav-item>
         <b-nav-item href="#">Course</b-nav-item>
          <b-nav-item href="#">Videos</b-nav-item>
           <b-nav-item href="#">History</b-nav-item>
            <b-nav-item href="#">Online-classes</b-nav-item>
             <b-nav-item href="#">Contact us</b-nav-item>
      </b-navbar-nav>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
    </div>
    <router-view />
  </div>
</template>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #131416;
}

#nav {
 background-color: #2c358a;
}

#nav a {
  font-weight: bold;
  color: white;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
