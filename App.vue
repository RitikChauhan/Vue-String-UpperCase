<template>
  <div id="app">
    <span>Enter String Below:</span>
    <br>
    <textarea v-model="message" placeholder="You can add multiple lines"></textarea>
    <p>{{myStr2}}</p>
    <button @click="changeCase()">Change String Case</button>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data(){
    return{
      message:"",
      myStr2:""
    }
  },
  methods :{
    changeCase : function(){
      this.myStr2 = this.message.toUpperCase();
    }
  }
}
</script>

<style>
</style>
