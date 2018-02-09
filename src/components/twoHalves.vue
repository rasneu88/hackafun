<template>
  <div class="hello">
    <h1>{{ title }}</h1>
    <div class="container">
      <div class="text">
        <p>{{firstText}}</p>
        <p>{{secondText}}</p>
        <a v-bind:href="link">{{CAT}}</a>
      </div>
      <div class="img-wrapper">
        <img :src="img" alt="">
    </div>

    </div>
  </div>
</template>

<script>

export default {
  name: 'twoHalves',
  props: ['type'],
  data () {
    return {
      title: 'This is your section with two halves',
      firstText: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exero eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore ',
      secondText: 'Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea cnim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore',
      CAT: 'Click here for even more soup',
      link: 'http://www.countryliving.com/soup-recipes/',
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
  margin:1rem;
}

.text {
  width: 50%;
  overflow-y:auto;
  margin:1rem;

}

.text p {
  margin-bottom:4rem;
}

.text p:nth-child(odd) {
  margin-left:1rem;
  padding-left:1rem;
  border-left:solid 5px darkred;
}
.text p:nth-child(even) {
  margin-right:1rem;
  padding-right:1rem;
  border-right:solid 5px #7c7c7c;
}
.text a {
  text-decoration: none;
  color: darkred;
  font-weight: bold;
}

.img-wrapper {
  width: 50%;
}
  img {
    width:100%;
    padding:1rem;


  }


</style>
