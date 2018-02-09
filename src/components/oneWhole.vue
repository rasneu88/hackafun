<template>
  <div class="container">
    <h1 class="headline">{{ msg }}</h1>
    <div class="circle"></div>
    <div class="text-box">
      <p class="text-box__first-text">
        {{firstMessage}}
      </p>
      <p class="text-box__second-text">
        {{secondMessage}}
      </p>
    </div>
    <div class="circle"></div>
  </div>
</template>

<script>
  export default {
    name: 'oneWhole',
    data() {
      return {
        msg: 'Here is your full size section',
        imgSrc: '/static/logo.png',
        firstMessage:
              'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam felis justo, bibendum ut velit vel, interdum ultricies mauris. Integer ut turpis et enim finibus placerat. Integer sed interdum diam, sit amet elementum leo. Proin risus eros, cursus at orci at, commodo euismod lectus. Donec nisl massa, facilisis eu eros et, porttitor ultricies dui. Cras eu tristique massa, sed lacinia orci.',
        secondMessage:'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam felis justo, bibendum ut velit vel, interdum ultricies mauris. Integer ut turpis et enim finibus placerat. Integer sed interdum diam, sit amet elementum leo. Proin risus eros, cursus at orci at, commodo euismod lectus. Donec nisl massa, facilisis eu eros et, porttitor ultricies dui. Cras eu tristique massa, sed lacinia orci.',
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .container {
    background-color: grey;
    padding: 2rem 0 2rem 0;
    margin:1rem;
  }

  .headline {
    margin: 0 0 2rem 0;
    color: white;
  }

  .text-box {
    display: flex;
    flex-wrap:wrap;
    justify-content: center;
  }
  .text-box p {
    border-color:darkgoldenrod;
    color:white;
    flex-shrink: 0;
    width: 70%;
    padding:1rem;
    font-family: "Agency FB";
    letter-spacing: 1px;
    font-size:1.5rem;
  }

  .text-box__first-text {
    border-left: solid 5px;
  }
  .text-box__second-text {
    border-right: solid 5px;
  }

  .circle {
    background-color:darkgoldenrod;
    border-radius: 50%;
    height:50px;
    width:50px;
    margin-left:auto;
    margin-right:auto;
  }
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
