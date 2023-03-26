<script>
    export default {
    data() {
        return {
        awesome: true
        }
    },
    methods: {
        toggle() {
            if(this.awesome === true){
                this.awesome = false;
            }else{
                this.awesome = true;
            }
        }
    }
    }
</script>

<template>
  <button @click="toggle">toggle</button>
  <h1 v-if="awesome">Vue is awesome!</h1>
  <h1 v-else>Oh no 😢</h1>
</template>