<template>
    <!-- regular way -->
    <Form>
        <label>Input here: </label>
        <input :value="text" @input="onInput" placeholder="Type here">
    </Form>
    <p>{{ text }}</p>
  </template>

<script>
    export default{
        data: function(){
            return { text: ''};
        },
        methods: {
            onInput(e) {
                // set text of Input to
                // value entered by user
                this.text = e.target.value;
            }
        }

    }

</script>

<style>
    input {
        margin: 10px;
    }
</style>