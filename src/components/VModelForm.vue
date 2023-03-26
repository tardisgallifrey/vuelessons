<template>
    <Form>
        <label>V-model Input:</label>
        <input v-model="text" placeholder="Type here"/>
    </Form>
    <p>{{ text }}</p>
</template>

<script>
//export is still required with v-model
//my guess is that it defines the variable
    export default {
        data: function(){
            return { text: ''};
        }
    }
</script>

<style>
    input {
        margin: 5px;
    }
</style>