<template>
    <section class="tt">
        <titulo-temp :title="titulo" class="fundoRGB"/>

        <br><br>

        <cards-shaders :title="titulo" :items="items"/>

    </section>
</template>

<style lang="scss">
    .fundoRGB .ttc{
        background: linear-gradient(180deg, #a47fb1, #76587a)!important;        
    }
</style>

<style lang="scss"  scoped>

   

    .tt{
        padding: 0 60px;

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
        // background: url("../static/imgs/fundo-titulo-shader.png");
        background: linear-gradient(180deg, #967fb1, #67577a);
        text-align: center;

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

    .card{
        border-color: rgb(230, 230, 230);

        .card-text{
            max-width: 500px;
            padding-top: 5px;
            line-height: 28px;
        }
    }

    .links{
        text-decoration: none;
        color: black;
    }

    .cat{
        text-decoration: none;
        color: black;
        background-color: rgb(205, 205, 205);
        padding: 5px;
        border-radius: 15px;
        font-size: 13px;
    }
</style>



<script>

    export default{
    // data vai armazenar as variaveis e os karai a 4
    data(){
      return{
        titulo : "Shaders",
        subtitulo : "Clique para ver mais",
        items: [
            {
                title: "BSL Shaders",
                img: "imgs/shader1.png",
                tags: ['Shader', 'Leve', 'Realista']
            },
            {
                title: "Chocapic13's Shaders",
                img: "imgs/shader2.png",
                tags: ['Shader', 'Leve', 'Realista']
            },
            {
                title: "Builders QOL Shaders",
                img: "imgs/shader3.png",
                tags: ['Shader', 'Leve', 'Realista']
            },
        ]
      }
    }
  }
</script>
<!-- 
<script>

  export default {
  
    setup() {
      const onSwiper = (swiper) => {
        console.log(swiper);
      };
      const onSlideChange = () => {
        console.log('slide change');
      };
      return {
        onSwiper,
        onSlideChange,
      };
    },
  };
</script> -->