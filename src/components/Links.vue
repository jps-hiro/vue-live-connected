<template>
    <nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" href="/">
      <img :src="image" class="nav-logo">
    </a>

    <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu">
    <div class="navbar-end">
      <a href="#work" class="navbar-item">Work</a>
      <a href="#play" class="navbar-item">Play</a>
      <a href="#innovate" class="navbar-item">Innovate</a>
    </div>
  </div>
</nav>

</template>

<script>
export default {
    data: () => ({
        image: require('../assets/img/connected_logo.png')
    })
}
</script>