<template>
  <div class="hello">
    <h1>{{ title }}</h1>

    <a href class="add-new-section">+</a>

    <div v-for="section in sections" :key="section.id">
      <two-halves/>
    </div>

  </div>
</template>

<script>
import twoHalves from './twoHalves'

export default {
  name: 'container',
  components: {
    twoHalves
  },
  data () {
    return {
      title: 'container title :)',
      sections: [
        {
          title: 'title for section 1',
          text: 'text for section 1',
          img: 'static/soup.jpg',
          template: 'twoHalves'
        },  
        {
          title: 'title for section 2',
          text: 'text for section 2',
          img: 'static/soup.jpg',
          template: 'oneWhole'
        },
        {
          title: 'title for section 3',
          text: 'text for section 3',
          img: 'static/soup.jpg',
          template: 'twohalves'
        },
        {
          title: 'title for section 4',
          text: 'text for section 4',
          img: 'static/soup.jpg',
          template: 'oneWhole'
        }                                          
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
