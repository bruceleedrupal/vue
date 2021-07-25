<template>
  {{title}}
  <input ref="name"/>
  <button @click="clickhandle">clickme</button>
  <Modal/>
</template>

<script>
 
 import Modal from "./components/Modal.vue";


export default {
  name: 'App',
  components:{Modal},
  data(){
    return {
      title:'My first app'
    }
  },
  methods:{
    clickhandle(){
      console.log(this.$refs.name);
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
