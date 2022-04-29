<template>

    <div :class="Estilo">
        <div class="shape1"></div>
        <div class="shape2"></div>
        <div class="shape3"></div>
        <div class="shape4"></div>
        <div class="shape5"></div>
    </div>
  
</template>

<script>
export default {
    name: 'BackgroundShapes',
    props:{
        Estilo: String,
    }
}
</script>

<style>

    .dark{
        background-color: black;
    }

    /* ESTILO SPRING */

    .Spring{
        width: 100%;
        height: 100%;
        min-height: 640px;

        position: relative;
    }

    .Spring .shape1{
        background-color: #A5CAD2;
        box-shadow: 0 0 15px #A5CAD2,
                0 0 100px #A5CAD2;
        border: 2px solid white;
        width: 75px;
        height: 150px;
        border-radius: 100px 0 0 100px;
        
        position: absolute;
        right: 1%;
        top: 3%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Spring .shape1:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    .Spring .shape2{
        background-color: #FF7B89;
        box-shadow: 0 0 15px #FF7B89,
                0 0 100px #FF7B89;
        border: 2px solid white;
        width: 180px;
        height: 450px;
        border-radius: 100px 100px 100px 0;

        position: absolute;
        right: 1%;
        bottom: 2%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Spring .shape2:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    .Spring .shape3{
        background-color: #8A50B2;
        box-shadow: 0 0 15px #8A50B2,
                0 0 100px #8A50B2;
        border: 2px solid white;
        width: 150px;
        height: 175px;
        border-radius: 100px 100px 100px 100px;

        position: absolute;
        left: 1%;
        top: 20%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Spring .shape3:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    .Spring .shape4{
        background-color: #6F5F90;
        box-shadow: 0 0 15px #6F5F90,
                0 0 100px #6F5F90;
        border: 2px solid white;
        width: 350px;
        height: 150px;
        border-radius: 0 100px 0 100px;

        position: absolute;
        right: 16%;
        bottom: 2%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Spring .shape4:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    .Spring .shape5{
        background-color: #758EB7;
        box-shadow: 0 0 15px #758EB7,
                0 0 100px #758EB7;
        border: 2px solid white;
        width: 150px;
        height: 150px;
        border-radius: 100px 0 100px 100px;

        position: absolute;
        top: 3%;
        left: 6%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Spring .shape5:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    /* ESTILO SUMMER */

    .Summer{
        width: 100%;
        height: 100%;
        min-height: 640px;

        position: relative;
    }

    .Summer .shape1{
        background-color: #35BBCA;
        box-shadow: 0 0 15px #35BBCA,
                0 0 100px #35BBCA;
        border: 2px solid white;
        width: 75px;
        height: 150px;
        border-radius: 100px 0 0 100px;
        
        position: absolute;
        right: 1%;
        top: 3%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Summer .shape1:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    .Summer .shape2{
        background-color: #FE7A15;
        box-shadow: 0 0 15px #FE7A15,
                0 0 100px #FE7A15;
        border: 2px solid white;
        width: 180px;
        height: 450px;
        border-radius: 100px 100px 100px 0;

        position: absolute;
        right: 1%;
        bottom: 2%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }
    
    .Summer .shape2:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    .Summer .shape3{
        background-color: #0191B4;
        box-shadow: 0 0 15px #0191B4,
                0 0 100px #0191B4;
        border: 2px solid white;
        width: 150px;
        height: 175px;
        border-radius: 100px 100px 100px 100px;

        position: absolute;
        left: 1%;
        top: 20%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Summer .shape3:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    .Summer .shape4{
        background-color: #F8D90F;
        box-shadow: 0 0 15px #F8D90F,
                0 0 100px #F8D90F;
        border: 2px solid white;         
        width: 350px;
        height: 150px;
        border-radius: 0 100px 0 100px;

        position: absolute;
        right: 16%;
        bottom: 2%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Summer .shape4:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

    .Summer .shape5{
        background-color: #D3DD18;
        box-shadow: 0 0 15px #D3DD18,
                0 0 100px #D3DD18;
        border: 2px solid white; 
        width: 150px;
        height: 150px;
        border-radius: 100px 0 100px 100px;

        position: absolute;
        top: 3%;
        left: 6%;

        -webkit-transform: translateY(0);
        -moz-transform: translateY(0);
        -ms-transform: translateY(0);
        -o-transform: translateY(0);
        transform: translateY(0);
        -webkit-transition: 0.5s;
        -o-transition: 0.5s;
        -moz-transition: 0.5s;
        transition: 0.5s;
    }

    .Summer .shape5:hover{
        -webkit-transform: translateY(-8px);
        -moz-transform: translateY(-8px);
        -ms-transform: translateY(-8px);
        -o-transform: translateY(-8px);
        transform: translateY(-8px);
    }

</style>