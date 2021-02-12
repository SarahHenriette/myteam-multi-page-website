<template>
    <nav id="nav" class="background-midnight-green">
        <div class="nav-principal">
            <span id="logo"><router-link to="/"><img src="images/logo.svg" alt="logo de my team"></router-link></span>
            <ul class="links-home-about">
                <li><router-link to="/">home</router-link></li>
                <li><router-link to="/about">about</router-link></li>
            </ul>
        </div>
        <ul class="link-contact">
            <li class="btn normal-state-light"><router-link to="/contact">contact us</router-link></li>
        </ul>
        <div class="nav-mobile">
            <svg  @click="displayMenuResponsive" xmlns="http://www.w3.org/2000/svg" width="20" height="17"><g fill="#FFF" fill-rule="evenodd"><path d="M0 0h20v3H0zM0 7h20v3H0zM0 14h20v3H0z"/></g></svg>
        </div>
        <div @click="hideMenuResponsive" :class="responsive" class="background-menu-nav-mobile"></div>
        <div :class="responsive" class="menu-nav-mobile" id="menu-nav-mobile">
            <svg @click="hideMenuResponsive" class="close" xmlns="http://www.w3.org/2000/svg" width="18" height="17"><path fill="#FFF" fill-rule="evenodd" d="M15.01.368l2.122 2.122-6.01 6.01 6.01 6.01-2.122 2.122L9 10.622l-6.01 6.01L.868 14.51 6.88 8.5.87 2.49 2.988.368 9 6.38 15.01.37z"/></svg>
            <ul class="links-home-about-mobil">
                <li @click="hideMenuResponsive"><router-link to="/">home</router-link></li>
                <li @click="hideMenuResponsive"><router-link to="/about">about</router-link></li>
            </ul>
             <ul class="link-contact-mobile">
                <li @click="hideMenuResponsive" class="btn normal-state-light"><router-link to="/contact">contact us</router-link></li>
            </ul>
            <svg xmlns="http://www.w3.org/2000/svg" class="background-image" width="200" height="200"><g fill="none" fill-rule="evenodd"><path fill="#2C6269" d="M100 100H0V0h100z"/><path fill="#F67E7E" d="M100 0c55.228 0 100 44.772 100 100s-44.772 100-100 100S0 155.228 0 100 44.772 0 100 0zm0 67c-18.225 0-33 14.775-33 33s14.775 33 33 33 33-14.775 33-33-14.775-33-33-33z"/><path fill="#79C8C7" d="M100 40v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0V8h100zm0-8v4H0V0h100z"/></g></svg>
        </div>
    </nav>
</template>

<script>
export default {
    data () {
        return {    
            responsive: ""
        }
    }, 
    methods : {
        displayMenuResponsive() {
            this.responsive = "active"
        },
        hideMenuResponsive() {
            this.responsive = ""
        }
    }
}
</script>
    

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
    .nav-principal {
        display: flex;
        align-items: center;
        #logo {
            list-style-type: none;
        }
        .links-home-about {
            margin-left: 80px;
            width: 140px;
            height: 28px;
            display: flex;
            justify-content: space-between;
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
    .active {
        display: flex!important;
    }
    .background-menu-nav-mobile {
        width: 375px;
        height: 667px;
        background-color: $darkGreen;
        opacity: 0.8;
        position: absolute;
        top: -48px;
        left: -24px;
        display: none;
    }
    .menu-nav-mobile {
        width: 255px;
        height: 667px;
        background-color: $midnightGreen;
        position: absolute;
        right: -24px;
        top: -48px;
        z-index: 5;
        display: none;
        flex-direction: column;
        animation: display 1s ease;
        .close {
            position: absolute;
            right: 25px;
            top: 56px;
        }
        .background-image {
            position: absolute;
            bottom: 0;
            right: -100px;
        }
        .links-home-about-mobil {
            display: flex;
            flex-direction: column;
            position: absolute;
            top: 112px;
            left: 48px;
            li {
                margin-bottom: 24px;
            }
            margin-bottom: 36px;
        }
        .link-contact-mobile {
            position: absolute;
            top: 228px;
            left: 48px;
        }
    }

    @keyframes display {
        0% { right : -279px }
        100%{ right : -24px }
    }
    @keyframes hide {
        0% { right : -24px }
        100%{ right : -279px }
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
