<template>
    <section>
        <button @click="buttonclick()">{{botao}}</button>
        <img :src="farofa" :alt="nome" :style="a">
        <p>{{nome}}</p>
        <h3>
            {{abacate}}
        </h3>
    </section>
</template>

<script>
  export default{
    // data vai armazenar as variaveis e os karai a 4
    data(){
      return{
        nome : "alguma coisa",
        botao : "oi",
        farofa : "imgs/mine.png"
      }
    },

    props: {
        abacate: {
            default: "abacate verde",
            type: String,
        }
    },

    // coisinho q faz funfa assim q recarrega a pagina
    // mounted(){
    //     this.buttonclick()
    // },
    
    // methods, é pra por varias funções juntinha
    methods:{
        buttonclick(){
            console.log("oaruhg")

            this.nome = "outra coisa"
            this.botao = "tchau"
            this.farofa = "imgs/minespace.png"
        }
    }
  }


</script>