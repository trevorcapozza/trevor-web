<template>
  <div>
    <div class="topline"></div>
    <div class="navbar max">
      <h2><span>trevor</span>capozza</h2>
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

<style lang="scss" scoped>

.topline {
  border-top: 10px solid #0074d9;
}

h2 {
  font-size: 30px;
  font-weight: 500;

  span {
    font-weight: 900;
    color: #0074d9
  }
}

.nav-links {
  font-size: 18px;
  display: flex;
  align-items: center;
}

.navbar {
  margin: 25px auto 175px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 40px;

  a {
    font-weight: 700;
    color: #8f9ea5;
    text-decoration: none;
    cursor: pointer;

    &.router-link-exact-active {
      color: #0074d9;
    }
    
    &:hover {
      color: #0074d9;
    }
    &:first-child {
      margin-right: 25px;
    }
  }
}


@media screen and (max-width: 560px) {

.logo {
  width: 225px;
}

.navbar {
  flex-direction: column;
  margin-bottom: 100px; 
  a {
    margin: 20px 0px;
    font-weight: 500;
  }
}

h2 span {
  font-weight: 700;
}

}

</style>