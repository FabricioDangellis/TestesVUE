<template>

    <div :class="Tema">
        <div class="container">
            
            <h1>Faça o <strong>Login</strong> na sua conta</h1>
            <div class="dadoslogin">
                <input-type id="email" Type="email" msg="Digite seu email" />
                <input-type id="senha" Type="password" msg="Digite sua senha" />
            </div>
            <bottonStyle v-on:dados-logar="logar" Estilo="blue" Texto="Entrar"/>
            
        </div>
    </div>

</template>

<script>
import bottonStyle from './buttonStyle.vue'
import inputType from './inputType.vue'


export default {
    components: { inputType, bottonStyle },

    name: 'loginLayout',

    props: {
        Tema: String,
    },

    methods: {

        logar() {
            let email = document.getElementById("email").value;
            let senha = document.getElementById("senha").value;

            if(!email){
                alert("Campo de email não preenchido!");
            }
            else{
                if(!senha){
                    alert("Campo de senha não preenchido!");
                }
                else{
                    alert("Logado no sistema");
                }
            }
        }

    }

}
</script>

<style>

    .dadoslogin{
        width: 500px;
        margin-top: 40px;
        margin-bottom: 20px;
    }

    .Light h1{
        margin-top: 20px;
        color: #000;
    }

    .Light strong{
        color: red;
    }

    .Dark h1{
        margin-top: 20px;
        color: #fff;
    }
    
    .Spring strong{
        color: #FF7B89;
    }

    .Summer strong{
        color: #D3DD18;
    }

    .Dark .container{
    width: 500px;
    height: 500px;
    background-color: #111113;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
    position: absolute;
    top: 50%;
    left: 50%;
    margin: -250px 0 0 -250px;

    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  }

</style>