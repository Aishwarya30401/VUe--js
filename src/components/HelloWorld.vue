<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  <form>
    <label> {{age}}   </label>
    <label>Name :</label>
    <input type="text" placeholder="enter your name"> 
    <br>
    <br>
    <label> E-mail :</label>
    <input type="text" placeholder="enter your mail"> 
    <br>
    <br>
    <label>Mobile No: </label>
      <input type="text" placeholder="enter your mobile number">
    </form>
    <br>
    <br>
  <button @click="increment">count is: {{ count }}</button>
  </div>
</template>

<script>

export default {
  data() {
    return {
      count: 0
    }
  },
  methods: {
    increment() {
      // update component state
      this.count++
    }
  }
}



</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button{
  width:170px;
  height:30px;
  border:2px solid gray;
  color:black;
  margin-left:100px;
}
</style>
