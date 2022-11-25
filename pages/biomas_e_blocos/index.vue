<template>
    <section>
        <div>
            <div>
                <figure v-for="(item, index) in bioblock[0]" :key="index" @click="gelatina = index">
                    <img  :src="item" alt="">
                </figure>
                <div v-for="(item, index) in bioblock[1]" :key="index">
                    <figure v-if="gelatina == index">
                        <img :src="item" alt="">
                    </figure>
                </div>
                <!-- <figure v-for="(item, index) in bioblock[1]" :key="index">
                    <img :src="item" alt="">
                </figure> -->
            </div>
        </div>
    </section>
</template>

<script>

    export default {
        data() {
            return{
                blocos : ["imgs/Grass_Block.png", "imgs/Red_Sand.png", "imgs/Snow_Block.png" ,"imgs/Netherrack.png", "imgs/End_Stone.png"],
                biomas : ["imgs/Plains.png", "imgs/Badlands.png", "imgs/Icy_Tundra.png", "imgs/Nether.png", "imgs/The_End.png"],
                bioblock: [],
                gelatina : 0
            }
        },

        mounted(){
            this.bioblock.push(this.blocos, this.biomas);
            this.syncArray();
        },

        methods: {
            // tem q fazer função p juntar dois array, e um array p imprimir os dois seja em console ou em texto
            syncArrayTest(){
                // for each pra cada item de dentro dos blocos
                this.blocos.forEach((item, index) => {
                        // variavel pro numero de cada array imprimir um bglh diferente, e o index soma automaticamente então não -
                        // precisa de calculo
                        var feijao = this.blocos[index] + ' = ' + this.biomas[index] 
                        this.bioblock.push(feijao)
                }
                )
            },
            syncArray(){
                
            }
        }
    }
</script>