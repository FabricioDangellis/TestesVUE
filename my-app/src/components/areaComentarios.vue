<template>

    <div class="area">
        <h1>{{ Titulo }}</h1>
        <hr>
        <div>
            <p>
                <input type="text" placeholder="Nome" class="nome" v-model="nome">
            </p>
            <p>
                <textarea placeholder="Comentário" class="corpocomentario" v-model="mensagem"></textarea>
            </p>
            <button type="submit" class="botao" v-on:click="adicionarComentario">Enviar</button>
        </div>
        <div>
            <div class="comentario" v-for="(comment, index) in comments" :key=" comment.id">
                <span>Autor: <strong>{{ comment.nome }}</strong></span>
                <p>{{ comment.mensagem }}</p>
                <div class="excluir">
                    <a href="#" v-on:click.prevent="excluirComentario(index)">Excluir</a>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: 'areaComentarios',

    props: {
        Titulo: String
    },

    data() {
        return {
            comments: [],
            nome: '',
            mensagem: '',
        }
    },

    methods: {

        adicionarComentario() {
            if(this.nome.trim() === ''){
                alert("Preenche sue nome");
                return;
            }
            else{
                if(this.mensagem.trim() === ''){
                    alert("Coloque um comentário");
                    return;
                }
                else{
                    this.comments.push({
                        nome: this.nome,
                        mensagem: this.mensagem
                    });

                    this.nome = '';
                    this.mensagem = '';
                }
            }

        },

        excluirComentario(index) {
            this.comments.splice(index, 1); /*o splice vai remover a partir da posiçao passada(no caso, uma posição a frente) */
        }
    }

}
</script>

<style>

    .area {
        width: 40%;
        min-width: 650px;
        margin: 20px auto;
    }

    .nome{
        width: 100%;
        height: 50px;
        margin:  10px 0;
        padding: 5px;
        font-size: 20px;
        border: 1px solid black;
    }

    .corpocomentario{
        width: 100%;
        height: 100px;
        margin:  10px 0;
        padding: 5px;
        font-size: 20px;
        border: 1px solid black;
    }

    .botao{
        width: 100px;
        font-size: 20px;
        padding: 5px;
        background: #5e72eb;
        border: 1px solid grey;
        color: #fff;
        cursor: pointer;
    }

    .comentario{
        width: 100%;
        height: 80px;
        margin-top: 10px;
        padding: 10px;
        border: 1px solid #828385;

        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    }

    .comentario p{
        margin-top: 10px;
    }

    .excluir {
        margin-top: 20px;
    }

    .excluir a{
         text-decoration: none;
    }

</style>
