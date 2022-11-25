<template>
    <section>
        <h1>Customização de Texto</h1>

        <button @click="changetext()">Mudar texto</button>
        <p>{{texto}}</p>
        <!-- <p>{{carro.nome}}</p>
        <img :src="carro.url" alt=""> -->
        <div v-for="(item, index) in vestimenta" :key="index">
            <div>
                <h1>
                    {{item}}
                </h1>
                <img v-if="item == 'bermuda' " src="imgs/mine.png" alt="">
            </div>
        </div>
        <div class="texto1" v-if="texto == 1">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam alias illo at dolorum magni voluptates eveniet, nostrum harum ducimus animi similique quisquam temporibus reprehenderit sint minus aperiam culpa veritatis amet.
        </div>
        <div class="texto2" v-if="texto == 2">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam alias illo at dolorum magni voluptates eveniet, nostrum harum ducimus animi similique quisquam temporibus reprehenderit sint minus aperiam culpa veritatis amet.
        </div>
        <div class="texto3" v-else>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam alias illo at dolorum magni voluptates eveniet, nostrum harum ducimus animi similique quisquam temporibus reprehenderit sint minus aperiam culpa veritatis amet.
        </div>
    </section>
</template>

<style lang="scss" scoped>
    .texto1{
        color: red;
        background-color: black;
    }
    .texto2{
        color: yellow;
        background-color: black;
    }
    .texto3{
        color: cyan;
        background-color: black;
    }
</style>

<script>


    export default{
        data(){
         return{
            texto : 3,
            vestimenta : ["blusa", "sapato", "bermuda", "toca"],
            carro : { 
                nome : "Carlos",
                cor : "Amarelo",
                modelo : "Camaro",
                placa : "BTS2022",
                url : "imgs/mine.png",
                num : 4
            }
         }
        },

        mounted(){
            this.loop()
        },

        methods:{
            changetext(){
                if(this.texto == 1 ){
                    this.texto = 2
                }
                else if(this.texto == 2){
                    this.texto = 1
                }
            },
            loop(){
                for(let contador = 0; contador < this.vestimenta.length; contador = contador + 1) console.log(this.vestimenta[contador]);
                    // this.vestimenta[2]
                // this.vestimenta.forEach((item) => console.log(item))

                // console.log(this.vestimenta);
            }
      
        }
    }
    
</script>