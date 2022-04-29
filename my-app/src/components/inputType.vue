<template>

    <input class="inputType" :type="Type" :placeholder="msg">

</template>

<script>

export default {
   nome:'inputType',
   props: {
       msg: String,
       Type: String
   }
}

</script>

<style>

    .inputType{
        font-size: 20px;
        background-color: white;
        border: 2px solid black;
        border-radius: 20px;
        width: 65%;
        height: 25px;
        margin: 10px auto;
        padding: 5px;
        display: block;
    }

</style>