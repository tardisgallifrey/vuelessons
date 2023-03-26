<script>
    //returns title css class name to 
    //all v-bind div's with titleClass value
    export default {
    data() {
        return {
        titleClass: 'title'
        }
    }
    }
</script>

<template>
    <!-- v-bind used in HTML -->
  <div v-bind:id="dynamicId">
    <!-- So common is v-bind, that it can be dropped -->
    <h1 :class="titleClass">Make me red</h1>
  </div>

</template>

<style>
.title {
  color: red;
}
</style>