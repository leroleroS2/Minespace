<template>
    <section class="tt">
        <titulo-temp :title="titulo"/>

        <br><br>

        <cards-texturas :title="titulo" :items="items"/>
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

    // .cards{
    //     background-image: linear-gradient(to right, #ffffff, #f8f8f8, #f0f0f0, #e9e9e9, #e2e2e2, #e2e2e2, #e2e2e2, #e2e2e2, #e9e9e9, #f0f0f0, #f8f8f8, #ffffff);
    // }

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
        titulo : "Texturas",
        subtitulo : "Clique para ver mais",
        items: [
            {
                title: "LB Photo Realism Texture Pack",
                img: "imgs/textura1.jpeg",
                tags: ['Textura', 'Pesada', 'Realista', 'Detalhada']
            },
            {
                title: "Chocapic13's Shaders",
                img: "imgs/textura2.jpeg",
                tags: ['Textura', 'Leve', 'Simples', 'PvP', '+FPS']
            },
            {
                title: "Builders QOL Shaders",
                img: "imgs/textura3.jpeg",
                tags: ['Textura', 'Realista', 'Construção', 'Moderna', 'Decoração',]
            },
        ]
      }
    }
  }

//   export default {
  
//     setup() {
//       const onSwiper = (swiper) => {
//         console.log(swiper);
//       };
//       const onSlideChange = () => {
//         console.log('slide change');
//       };
//       return {
//         onSwiper,
//         onSlideChange,
//       };
//     },
//   };
</script>