<template>
  <div class="hello">
    <h1>{{msg}}</h1>
    <h3>count : {{count}}</h3>
    <button @click= "Increment">Increment</button>
    <button @click= "Decrement">Decrement</button>
    <button @click="Reset">Reset</button>


  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
      count : 0,
    }
  },
  methods : {
    Increment(){
      this.count += 1;
    },
    Decrement(){
      this.count -=1
    },
    Reset(){
      this.count = 0
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
