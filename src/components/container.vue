<template>
  <div class="hello">
    <h1>{{ title }}</h1>

    <a href class="add-new-section">+</a>

    <div v-for="section in sections" :key="section.id">
      <component :is="section.template"/>
    </div>
  </div>
</template>

<script>
import twoHalves from './twoHalves'
import oneWhole from './oneWhole'

export default {
  name: 'container',
  components: {
    twoHalves,
    oneWhole
  },
  data () {
    return {
      title: 'HackaFUN alla vue',
      sections: [
        {
          template: 'twoHalves'
        },
        {
          template: 'oneWhole'
        },
        {
          template: 'twoHalves'
        },
        {
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
