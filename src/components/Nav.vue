<template>
    <nav id="nav" class="background-midnight-green">
        <ul class="nav-principal">
            <li id="logo"><router-link to="/"><img src="images/logo.svg" alt=""></router-link></li>
            <ul class="links-home-about">
                <li><router-link to="/">home</router-link></li>
                <li><router-link to="/about">about</router-link></li>
            </ul>
        </ul>
        <ul class="link-contact">
            <li class="btn normal-state-light"><router-link to="/contact">contact us</router-link></li>
        </ul>
        <div class="nav-mobile">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="17"><g fill="#FFF" fill-rule="evenodd"><path d="M0 0h20v3H0zM0 7h20v3H0zM0 14h20v3H0z"/></g></svg>
        </div>
    </nav>
</template>
    

<style lang="scss">
    @import './public/sass/colors.scss';
    #nav {
        width: 1110px;
        height: 48px;
        background-color: $midnightGreen;
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: auto;
        position: absolute;
        top: 73px;
        left: 0;
        right: 0;
        z-index: 5;
        ul {
            display: flex;
            align-items: center;
            margin: 0;
            padding: 0;
            #logo {
                margin-right: 80px;
            }
            .links-home-about {
                li {
                    margin-right: 40px;
                }
            }
            li {
                list-style: none;
            }
            li a {
                text-decoration: none;
                color: $white;
                font-size: 18px;
                font-weight: 600;
                transition: color ease .5s;

            }
            li a:hover {
                color: $lightCoral;
            }
        }
        .link-contact {
            li {
                cursor: pointer;
                                transition: background-color ease .5s;

            }
                li:hover {
                    background-color: $white;
                    a {
                        color: $midnightGreen;
                    }
                }
            }
        .nav-mobile {
            display: none;
        }
    
    }

    @media screen and (max-width: 1390px) {
        #nav {
            width: 689px;
            ul #logo {
                margin-right: 48px;
            }
        }
    }
    @media  screen and (max-width: 759px) {
        #nav {
            width: 463px;
            .nav-principal .links-home-about {
                display: none;
            }
            .link-contact {
                display: none;
            }
            .nav-mobile {
                display: block;
            }
        }
    }
    @media screen and (max-width: 734px) {
        #nav {
            width: 327px;
            height: 32px;
            top: 48px;
            .nav-principal {
                #logo {
                    img {
                        width: 128px;
                        height: 32px;
                    }
                }
            }
        }
    }
</style>
