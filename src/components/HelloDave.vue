<script>

//basic default for message to
//HTML element
//Vue uses {{ }} to surround
//elements
export default {
  //Not a JScript function declaration
  data(){
    return {
      message: 'Hello, Dave.'
    }
  }
}

</script>

<template>
  <!-- Template marks boundary of Vue component HTML -->
  <h1>New Message</h1>
  <h1>{{ message }}</h1>
  <h3>All JavaScript works as elements</h3>
  <h3>{{ message.split('').reverse().join('') }}</h3>

</template>
