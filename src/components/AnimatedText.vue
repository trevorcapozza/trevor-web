<template>
  <div class="hero max">
    <vue-typed-js 
      class="type" 
      :strings="['Front-end Developer.', 'UI Designer.', 'Data Scientist.']" 
      :loop="true" 
      :typeSpeed="50" 
      :backSpeed="50" 
      @onComplete="doSmth()">
      <h1>Digital Marketer.<br><span class="typing"></span><br>Creator.</h1>
    </vue-typed-js>
	</div>
</template>


<script>

export default {
  name: 'animated-text'
}

</script>

<style lang="scss">

.hero {
  margin: 0 auto;
}

.type {
  justify-content: center;
}


</style>