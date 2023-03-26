<script>

//default is acting as the component's
//state container

//OK, default is a JavaScript Object
//It has the properties:
//data:
//methods:
//probably others
export default {
    //data is name of item/property
    //value(?) is a function
    //Usually, this form of anonymous function
    //lambda functions () => not allowed
    data: function() {
      return {
        count: 0
      }
    },
    //adding a method/function
    methods: {
      increment: function() {
        // update component state
        this.count++;
      }
    }
  }
</script>
  

<template>
  <!-- v-on defines an event listener -->
  <!-- it's shorthand is @ -->
  <!-- I could have used @click -->
  <button v-on:click="increment">count is: {{ count }}</button>
</template>