<template>
    <section class="header-prjt">

        <container class="header-prjt__cont">

            <div class="row">
                <nav class="main-nav">

                    <div class="col-6 col-md-12">
                        <div class="logo">
                            <div class="logo__minespace">
                                <img src="imgs/minespace.png" alt="" style="max-width: 50vw; width: 100%">
                            </div>
                        </div>
                    </div>

                    <div class="col-6 col-md-6">
                        <figure>
                            <nuxt-link to="/biomas_e_blocos">
                                <img class="bloco" display="block" src="imgs/mine.png" alt="Home">
                            </nuxt-link>
                        </figure>
                    </div>

                    <div class="col-12 col-md-6">
                        <div class="wrap">
                            <div class="search">
                                <input type="text" class="searchTerm" placeholder="Digite aqui...">
                                <button type="submit" class="searchButton">
                                    <i class="fa fa-search"></i>
                                </button>
                            </div>
                        </div>
                    </div>

                    <ul class="main-nav__pags">
                        <li class="main-nav__pagsbttn">
                            <nuxt-link class="main-nav__link" to="/aba-skins">
                                Skins
                            </nuxt-link>
                        </li>
                        <li class="main-nav__pagsbttn subcategorias-div">
                            <nuxt-link class="main-nav__link" to="/aba-texturas">
                                Texturas
                                <div class="baixou">
                                    <ul class="submenu">
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                Mais Populares
                                            </nuxt-link>
                                        </li>
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                Mais Baixadas
                                            </nuxt-link>
                                        </li>
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                Realistas
                                            </nuxt-link>
                                        </li>
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                PvP (+FPS)
                                            </nuxt-link>
                                        </li>
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                Decoração Morderna
                                            </nuxt-link>
                                        </li>
                                    </ul> 
                                </div>
                            </nuxt-link>
                        </li>
                        <li class="main-nav__pagsbttn">
                            <nuxt-link class="main-nav__link" to="/aba-shaders">
                                Shaders
                            </nuxt-link>
                        </li>
                        <li class="main-nav__pagsbttn">
                            <nuxt-link class="main-nav__link" to="/aba-mods">
                                Mods
                                <div class="baixou">
                                    <ul class="submenu">
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                Mais Populares
                                            </nuxt-link>
                                        </li>
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                Mais Baixados
                                            </nuxt-link>
                                        </li>
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                Construção
                                            </nuxt-link>
                                        </li>
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                PvP (+FPS)
                                            </nuxt-link>
                                        </li>
                                        <li class="subcategorias">
                                            <nuxt-link class="sublinks" to="/aba-texturas">
                                                Decoração Morderna
                                            </nuxt-link>
                                        </li>
                                    </ul> 
                                </div>
                            </nuxt-link>
                        </li>
                        <li class="main-nav__pagsbttn">
                            <nuxt-link class="main-nav__link" to="/aba-modpacks">
                                Mod Packs
                            </nuxt-link>
                        </li>
                        <li class="main-nav__pagsbttn">
                            <nuxt-link class="main-nav__link" to="/sliderr">
                                Capas
                            </nuxt-link>
                        </li>
                    </ul>
                    </nav>
            </div>

           
        </container>
    </section>
</template>

<style lang="scss" scoped>

    .header-prjt{
        
        padding: 15px 25px;
        max-width: 100%;
        // overflow: hidden;
        // background: url(./imgs/fundo-header.png);
        background: url("../static/imgs/fundo-header.png");

        .search {
            width: 600px;
            position: relative;
            display: flex;

            .searchTerm {
                width: 100%;
                border: 3px solid #ffffff;
                border-right: none;
                padding: 5px;
                height: 55px;
                border-radius: 5px 0 0 5px;
                outline: none;
                color: #ffffff;
            }

            .searchTerm:focus{
                color: #000000;
            }

            .searchButton {
                width: 55px;
                height: 55px;
                border: 1px solid #ffffff;
                background: url("../static/imgs/search.png");
                text-align: center;
                color: #fff;
                border-radius: 0 5px 5px 0;
                cursor: pointer;
                font-size: 20px;
            }

            /*Resize the wrap to see the search bar change!*/
            .wrap{
                width: 30%;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
            }
        }

        &__cont{
        // display: flex;

        }

        .main-nav{
            display: flex;
            width: 100%;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;

            &__buscar{
                font-family: 'VT323', monospace;
                width: 500px;
                height: 50px;
                border: none;
            }
            

            &__pags{
                margin-top: 18px;
                padding-right: 25px;

                position: relative;
                flex-direction: row;
                width: auto;
                top: 0;
                display: flex;

                list-style: none;

                background: #999 url('https://i.ibb.co/rb2TWXL/bgbtn.png') center / cover;
                image-rendering: pixelated;
                border: 2px solid #000;

                &:hover .title {
                    background-color: rgba(100, 100, 255, .45);
                    text-shadow: 2px 2px #202013CC;
                    color: #FFFFA0;
                }

                &:active .title {
                    box-shadow: inset -2px -4px #0004, inset 2px 2px #FFF5;
                }
            }

            &__pagsbttn{
                padding: 0 20px;

                margin: 0;
                display: flex;
                flex-direction: row;
                list-style: none;
                padding: 0;

                
            }

            &__link{
                padding: 5px 25px;

                cursor: pointer;
                text-transform: uppercase;
                text-decoration: none;
                font-size: 28px;
                color: #000000; 
                font-family: 'VT323', monospace;
                letter-spacing: 1.1px;

                position: relative;
                display: block;
                transition: 0.5s;

                &::after {
                    position: absolute;
                    content: "";
                    top: 100%;
                    left: 0;
                    width: 100%;
                    height: 3px;
                    background: white;
                    transform: scaleX(0);
                    transform-origin: right;
                    transition: transform 0.5s;
                }

                &:hover {
                    color: white;
                }

                &:hover::after {
                    transform: scaleX(1);
                    transform-origin: left;
                }
            }
        }
    }
    .subcategorias-div{
        position: relative;

        &:hover .baixou{
            display: block;
        }
    }

    .baixou{
        position: absolute;
        height: 350%;
        width: 150%;
        top: 100%;
        left: -25%;
        background: #999 url('https://i.ibb.co/rb2TWXL/bgbtn.png') center / cover;
	    image-rendering: pixelated;
        border: 2px solid #000;
        display: none;
    }

    .submenu{
        font-size: 24px;
        list-style: none;
        padding: 0 5px;
    }

    .sublinks{
        color: white;
    }

    .logo{
        &__minespace{
            text-align: center;
        }
    }

    @media (max-width: 360px) {
        .header-prjt{
            display: flex;
            flex-direction: row-reverse;
            .search{
                flex-direction: column;
                width: 320px;
                

                .searchTerm{
                    display: none;
                }

                // .searchButton{
                // }
            }

            .main-nav{
                flex-direction: column;
                &__pags{
                    display: none;
                }
            } 
        } 
        
        .logo{
            &__minespace{
                // display: none;
                width: 100px;
            }
        }
        .bloco{
            width: 70px;
        }
    }
    
</style>