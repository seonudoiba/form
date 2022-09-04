<template>
  <div>
    <h2>Guess the a number from 1-100 to Know My Crush </h2>
    <h4>You have only {{attempt}} left </h4>
    <form >
      <h3>Guessed Number: {{guessed}}</h3>
      <label for="num"><b>Input a Number From 1-100 : </b></label>
      <input min="1" max="100" type="number" id="num" v-model="guessed"/>
      <button v-on:click="console.log('Hi')" type="submit" class="btn">Check</button>
    </form>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data() {
    return {
      attempt: 5,
      guessed:"",
      randomNum: 56,
      message: "Starr"
    }
  },
  components: {
  
  },
  methods: {
    submitb() {
      // attempt = this.attempt - 1
      // if(this.guessed == !this.randomNum){
      //   this.message = `You have ${this.attempt} left, Try again`
      // } else {
      //   this.message = "You CAn Now Know my crush"
      // }
      alert(`Hi ${attempt -1}`)
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 
  60px;
}
.btn{
  color: red;
}
</style>