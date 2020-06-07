<template>
<div>
  <div class="home">
    <h1 class="headline center">Blog</h1>
    <h4 class="small">This blog section is still under construction...</h4>
    <div class="sections">
      <div v-for="(section, index) in Object.keys(entries).slice().reverse()" :key="index" class="group">
        <!-- <h2 class="center">{{section}}</h2> -->
        <div class="section" v-for="entry in entries[section]" :key="entry.id">
          <div class="entry">
            <div class="heading">
              <h3 class="title" @click="$router.push({name: entry.id})">
                {{entry.title}}
              </h3>
              <p class="subtitle">{{entry.date}}</p>
            </div>
            <p class="description">{{entry.description}}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import BLOGENTRIES from '@/statics/data/blogs.json'
export default {
  name: 'home',
  components: {
  },
  computed: {
    entries() {
      return BLOGENTRIES
    }
  }
}

</script>