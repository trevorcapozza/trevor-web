<template>
<div class="blog-page">
  <div class="blogs markdown-body">
    <router-view />
    <router-link to="/blog" tag="a" class="back">&laquo; Back</router-link>
  </div>
</div>
</template>

<script>

export default {
    components: {
  },
}
</script>

<style src="@/css/github-markdown.css" lang="css"/>

