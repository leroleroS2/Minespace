<template>
    <section>
        <container>
            <a href="#" target="_blank" class="ttc2">
                <div class="ttc">
                <h1>{{title}}</h1>
                <h5>{{subtitulo}}</h5>
            </div>
            </a>
        </container>
    </section>
</template>

<style lang="scss" scoped >

    // :root{
    //     --degrade:  #7f9eb1
    // }
    .tt{
        padding: 50px 60px;

        a{
            text-decoration: none;
        }

        h1{
            font-family: 'VT323', monospace;
        }
    }
    .ttc{
        padding: 35px;

        color: white;
        background: linear-gradient(180deg, #7f9eb1, #586d7a);
        text-align: center;

        // url(../imgs/fundo-titulo-textura.png)

        text-decoration: none;

        .ttc::hover{
            text-decoration: none;
        }

        h1{
            font-size: 65px;
            font-family: 'VT323', monospace;
        }

        h5{
            font-size: 28px;
            font-family: 'VT323', monospace;
        }
    }

    .ttc2{

        color: white;
        text-align: center;

        text-decoration: none;

        .ttc::hover{
            text-decoration: none;
        }
    }
</style>

<script>
    export default{
    // data vai armazenar as variaveis e os karai a 4
    data(){
        return{
            titulo : "Texturas",
            subtitulo : "Clique para ver mais"
      }
    },

    props: {
        title: {
            type: String,
            default: "texto"
        }
    }
  }
</script>