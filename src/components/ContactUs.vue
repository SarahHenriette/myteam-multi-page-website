<template>
    <section class="contact-us">
        <div class="contain-text">
            <h2>Ready to get started?</h2>
            <li class="btn btn-contact-us"><router-link to="/contact">contact us</router-link></li>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" width="200" height="144"><g fill="none" fill-rule="evenodd"><path fill="#2C6269" d="M100 144H0V44h100z"/><path fill="#004047" d="M100 44c55.228 0 100 44.772 100 100s-44.772 100-100 100S0 199.228 0 144 44.772 44 100 44zm0 67c-18.225 0-33 14.775-33 33s14.775 33 33 33 33-14.775 33-33-14.775-33-33-33z"/><path fill="#F67E7E" d="M100 140v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100z"/><path fill="#79C8C7" d="M4 40v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zM4 32v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zM4 24v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm-35-8v4h-4v-4h4zm14 0v4h-4v-4h4zm-7 0v4h-4v-4h4zm21 0v4h-4v-4h4zm-7 0v4h-4v-4h4zM4 16v4H0v-4h4zm7 0v4H7v-4h4zm42 0v4h-4v-4h4zM4 8v4H0V8h4zm7 0v4H7V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zM4 0v4H0V0h4zm7 0v4H7V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4z"/></g></svg>
    </section>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
@import './public/sass/colors.scss';

.contact-us {
    width: 100%;
    height: 200px;
    background-color: $lightCoral;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    overflow: hidden;

    .contain-text {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 917px;
        height: 48px;

        h2 {
            color: $darkGreen;
            font-style: normal;
            font-weight: bold;
            font-size: 48px;
            line-height: 48px;
        }

        .btn-contact-us {
            background-color: $lightCoral;
            font-size: 18px;
            line-height: 28px;
            font-weight: 600;
            border-style: solid;
            border-color: $darkGreen;
            color: $darkGreen;
            cursor: pointer;
            transition: background-color ease .5s, color ease .5s;
            ;

            &:hover {
                background-color: $darkGreen;
                color: $white;
                a {
                    color: $white;
                }
            }

            a {
                color: $darkGreen;
                text-decoration: none;
                font-family: 'Livvic', sans-serif;
                font-size: 18px;
                font-weight: 600;
            }
        }
    }

    svg {
        position: absolute;
        bottom: 0;
        left: 0;
    }
}

@media screen and (max-width: 1120px) {
    .contact-us {
        .contain-text {
            width: 573px;

            h2 {
                font-size: 32px;
                line-height: 32px;
            }
        }

        svg {
            bottom: -22px;
        }
    }
}

@media screen and (max-width: 600px) {
    .contact-us {
        height: 302px;

        .contain-text {
            height: 136px;
            width: 327px;
            flex-direction: column;

            h2 {
                text-align: center;
                margin-top: 0;
                margin-bottom: 24px;
            }

            .btn-contact-us {
                padding: 9px 0 11px 0;
            }
        }
    }
}
</style>