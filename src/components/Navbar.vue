<template>
  <div>
    <div class="topline"></div>
    <div class="navbar max">
      <h2 class="logo"><span>trevor</span>capozza</h2>
      <!-- <img src="@/assets/logo.svg" alt="" class="logo"> -->
      <div class="nav-links">
        <router-link :to="{ name: 'Home' }">Home</router-link>
        <router-link :to="{ name: 'Blog' }">Blog</router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>
