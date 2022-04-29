<template>
    <div v-on:click="logar" :class="Estilo">
        <a>{{ Texto }}</a>
    </div>
</template>

<script>
export default {
    name: 'bottonStyle',
    props: {
        Texto: String,
        Estilo: String,
    },

    methods: {

        logar() {
            this.$emit('dados-logar', {})
        }

    }
}
</script>

<style >

    .day{
        display: flex;
        align-items: center;
        justify-content: center;
        width: 200px;
        height: 40px;
        border-radius: 20px;
        color: #fff;
        background: linear-gradient(to right,
                                #2a9d8f,
                                #FE7A15);
        box-shadow: 5px 5px 5px #696969;
        font-family: 'Nunito', sans-serif;
        font-size: 25px;
        cursor: pointer;
    }

     .blue{
        display: flex;
        align-items: center;
        justify-content: center;
        width: 200px;
        height: 40px;
        border-radius: 20px;
        color: #fff;
        background: linear-gradient(to right,
                                #00ffed,
                                #9d00c6);
        box-shadow: 5px 5px 5px #696969;
        font-family: 'Nunito', sans-serif;
        font-size: 25px;
        cursor: pointer;
    }

    .blue:hover{
        box-shadow: 5px 5px 5px #fff;
    }

    .day:hover{
        box-shadow: 5px 5px 5px #fff;
    }

    @import url('https://fonts.googleapis.com/css2?family=Nunito&display=swap')

</style>