<template>
  <div class="hello">
    <h1>{{ title }}</h1>
    <div class="container">
      <div class="text-left">
        {{txt}}
      </div>
      <div class="img-right">
        <img :src="img" alt="">
      </div>    
    </div>
  </div>
</template>

<script>

export default {
  name: 'twoHalves',
  data () {
    return {
      title: 'Two halves title',
      txt: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore ',
      img: 'static/soup.jpg'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

.container {
  display: flex;
}

.text-left {
  width: 50%;
}

.img-right {
  width: 50%;
}


</style>
