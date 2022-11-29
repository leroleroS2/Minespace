<template>
    <section class="header-prjt">

        <container class="logo">
            <div class="logo-minespace">
                <img src="imgs/minespace.png" alt="">
            </div>
        </container>

        <container class="header-prjt__cont">

            <nav class="main-nav">
                
                <figure>
                    <nuxt-link to="/biomas_e_blocos">
                        <img display="block" src="imgs/mine.png" alt="Home">
                    </nuxt-link>
                </figure>

                <div class="wrap">
                    <div class="search">
                        <input type="text" class="searchTerm" placeholder="Digite aqui...">
                        <button type="submit" class="searchButton">
                            <i class="fa fa-search"></i>
                        </button>
                    </div>
                </div>

                <ul class="main-nav__pags">
                    <li class="main-nav__pagsbttn">
                        <nuxt-link class="main-nav__link" to="/aba-skins">
                            Skins
                        </nuxt-link>
                    </li>
                    <li class="main-nav__pagsbttn">
                        <nuxt-link class="main-nav__link" to="/aba-texturas">
                            Texturas
                            <ul class="submenu" style="display: none;">
                                <li>
                                    Mais Populares
                                </li>
                                <li>
                                    Mais Baixadas
                                </li>
                                <li>
                                    Realistas
                                </li>
                                <li>
                                    PvP (+FPS)
                                </li>
                                <li>
                                    Decoração Morderna
                                </li>
                            </ul>
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
                        </nuxt-link>
                    </li>
                    <li class="main-nav__pagsbttn">
                        <nuxt-link class="main-nav__link" to="/aba-modpacks">
                            Mod Packs
                        </nuxt-link>
                    </li>
                    <li class="main-nav__pagsbttn">
                        <nuxt-link class="main-nav__link" to="/aba-capas">
                            Capas
                        </nuxt-link>
                    </li>
                </ul>
            </nav>
        </container>
    </section>
</template>

<style lang="scss" scoped>

    .logo{
        .logo-minespace{
            text-align: center;
        }
    }

    .header-prjt{
        padding: 15px 25px;
        max-width: 100%;
        overflow: hidden;
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
        display: flex;

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

    
</style>