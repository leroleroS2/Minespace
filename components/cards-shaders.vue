<template>
    <section>

        <container>
            <h1>- Mais populares : </h1><br>
        </container>

        <container class="cards">
            <div class="card-deck">
                <div v-for="(item, index) in items" :key="index" class="card">
                    <a href="#" target="_blank" style="text-decoration: none; color: black;"><img :src="item.img" class="card-img-top" alt="" href="#"></a>
                    <div class="card-body">
                        <h5 class="card-title">
                            <a href="#" target="_blank" class="links">{{item.title}}</a>
                        </h5>
                        <p class="card-text">
                            Version: 1.19.2 <br>
                            Categorias: <a v-for="(tag, index) in item.tags" :key="index"  href="#" target="_blank" class="cat">{{tag}}</a>
                        </p>
                    </div>
                </div>
            </div>
        </container>
    </section>
</template>

<style lang="scss" scoped >

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
        margin-right: 5px;
    }
</style>

<script>

    export default{
    // data vai armazenar as variaveis e os karai a 4
    data(){
      return{
        subtitulo : "Clique para ver mais"
      }
    },

    props: {
        title: {
            type: String,
            default: () => ""
        },
        items: {
            type: Array,
            default: () => []
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