<template>
    <div>
         <ul id="navegacao">
            <li class="n1 primeiro"> <a :href="link1"> {{ name1 }} </a> </li>
            <li class="n2"> <a :href="link2"> {{ name2 }} </a> </li>
            <li class="n3"> <a :href="link3"> {{ name3 }} </a> </li>
            <li class="n3"> <a :href="link4"> {{ name4 }} </a> </li>
            <li class="n5"> <a :href="link5"> {{ name5 }} </a> </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'navHorizontal',
    props: {
        name1: String,
        link1: String,
        name2: String,
        link2: String, 
        name3: String,
        link3: String,
        name4: String,
        link4: String, 
        name5: String,
        link5: String, 
    }
}
</script>

<style>

    ul{
    margin: 0;
    padding: 0;
    list-style: none;
    background: url(../assets/fundo-horizontal.png) repeat-x;
    float: left;
    }

    ul li{
        float: left;
    }

    ul a{
        display: block;
        padding: 0 2em;
        line-height: 2.2em;
        text-decoration: none;
        color: white;
        background: url(../assets/divisor.png) repeat-y left top;
    }

    ul .primeiro a{
        background: none;
    }

    ul a:hover{
        color: #085662;
        background: #44cade;
    }

    #home #navegacao .n1 a,
    #sobre #navegacao .n2 a,
    #servicos #navegacao .n3 a,
    #noticias #navegacao .n4 a,
    #contato #navegacao .n5 a{
        color: #085662;
        background: #44cade;
    }
</style>