<template>
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <HelloDave />
  <DynamicCSS />
  <ButtonCount />
  <MyForm />
  <VModelForm/>
  <ConditionalRender/>
</template>

<script>
//This whole file is a Single File Component (SFC)
//It contains the HTML, the JS, and the CSS (style)
//for one Vue Component

//This file is the ROOT component

//import another component
import HelloWorld from './components/HelloWorld.vue';

//Real tutorial begins in this component
import HelloDave from './components/HelloDave.vue';
import DynamicCSS from './components/DynamicCSS.vue';
import ButtonCount from './components/ButtonCount.vue';
import MyForm from './components/MyForm.vue';
import VModelForm from './components/VModelForm.vue';
import ConditionalRender from './components/ConditionalRender.vue';

//default export for this component
//with a list of imported components
export default {
  name: 'App',
  components: {
    HelloWorld,
    HelloDave,
    DynamicCSS,
    ButtonCount,
    MyForm,
    VModelForm,
    ConditionalRender
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
  background-color: darkgray;
  margin-top: 60px;
}
</style>
