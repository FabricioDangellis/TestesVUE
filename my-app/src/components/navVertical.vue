<template>
    <nav class="barra" id="Barra">
        <div class="fixa">
            <div class="menu" v-on:click="abrirMenu">
                <div class="linha"></div>
                <div class="linha"></div>
                <div class="linha"></div>
            </div>

            <ul class="lista">
                <li><a href=""><img src="../assets/bank-free-icon-font.png" alt=""></a></li>
                <li><a href=""><img src="../assets/info-free-icon-font.png" alt=""></a></li>
                <li><a href=""><img src="../assets/graduation-cap-free-icon-font.png" alt=""></a></li>
                <li><a href=""><img src="../assets/call-incoming-free-icon-font.png" alt=""></a></li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'navVertical',

    methods: {

        abrirMenu() {
            let barra = document.getElementById("Barra");
            let classBarra = barra.classList.contains("barraAberta");
            if(classBarra){
                barra.classList.remove("barraAberta");
            }
            else{
                barra.classList.add("barraAberta");
            }
        }
     }
    
}
</script>

<style>

    *{
        margin: 0;
        padding: 0;
    }

    .barra{
        background: #355c7d;
        width: 50px;
        height: 657px;
    }

    .barraAberta{
        width: 300px;
    }

    .fixa {
        width: 50px;
        height: 100%;
        color: #355c7d;
    }

    .menu{
        width: 40px;
        height: 35px;
        background: #355c7d;
        border-radius: 4px;
        padding-top: 3px;
        cursor: pointer;
        margin: auto;
    }

    .linha{
        background: #fff;
        width: 30px;
        height: 5px;
        margin: 3px auto;
        border-radius: 3px;
    }

    a{
        text-decoration: none;
        color: #fff;
    }

   .lista{
       list-style: none;
       margin: 40px auto;
    }

   .lista li {
       margin: 40px auto;
       width: 30px;
   }

    .lista img{
        width: 30px;
        height: 30px;
        margin: 10px auto;
    }
</style>