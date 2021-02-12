<template>
    <div class="testamonial">
        <div class="contain-text">
            <p class="text-testamonial">{{ text }}</p>
            <p class="name-telltale"> {{ name }} </p>
            <p class="profession-telltale">{{ profession }}</p>
            <div class="container-image">
                <img :src= img :alt= alt />
            </div>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" width="67" height="56"><path fill="#2C6269" d="M51.273 56c4.638 0 8.368-1.322 11.19-3.967 2.823-2.645 4.235-5.799 4.235-9.46 0-2.95-.429-5.494-1.286-7.63a197.251 197.251 0 01-2.495-6.562c-.806-2.237-1.21-4.933-1.21-8.087 0-2.746.454-5.798 1.361-9.155C63.976 7.782 65.286 4.069 67 0H55.356c-3.73 3.662-7.032 7.833-9.905 12.512-2.873 4.68-5.166 9.359-6.88 14.038C36.857 31.23 36 35.4 36 39.063c0 5.391 1.361 9.562 4.083 12.512C42.805 54.525 46.535 56 51.273 56zm-36 0c4.638 0 8.368-1.322 11.19-3.967 2.823-2.645 4.235-5.799 4.235-9.46 0-2.95-.429-5.494-1.286-7.63a197.251 197.251 0 01-2.495-6.562c-.806-2.237-1.21-4.933-1.21-8.087 0-2.746.454-5.798 1.361-9.155C27.976 7.782 29.286 4.069 31 0H19.356c-3.73 3.662-7.032 7.833-9.905 12.512-2.873 4.68-5.166 9.359-6.88 14.038C.857 31.23 0 35.4 0 39.063c0 5.391 1.361 9.562 4.083 12.512C6.805 54.525 10.535 56 15.273 56z"/></svg>
    </div>
</template>

<script>
export default {
    props: ["text", "name", "profession", "img", "alt"]
}
</script>

<style lang="scss" scoped>
  @import './public/sass/colors.scss';

.testamonial {
    width: 370px;
    height: 313px;
    position: relative;

    .contain-text {
        position: absolute;
        bottom: 0;
        z-index: 5;

        .text-testamonial {
            font-style: normal;
            font-weight: 600;
            font-size: 15px;
            line-height: 25px;
            text-align: center;
            color: $white;

        }

        .name-telltale {
            font-style: normal;
            font-weight: bold;
            font-size: 18px;
            line-height: 28px;
            text-align: center;
            color: $raptureBlue;
            padding-top: 24px;
        }

        .profession-telltale {
            font-style: italic;
            font-weight: 500;
            font-size: 13px;
            line-height: 18px;
            text-align: center;
            color: $white;
            padding-top: 2px;
            padding-bottom: 32px;
        }

        .container-image {
            height: 62px;
            width: 62px;
            border: 2px solid #C4FFFE;
            overflow: hidden;
            border-radius: 50%;
            margin: auto;

            img {
                width: 100%;
            }
        }
    }

    svg {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        margin: auto;
    }
}

@media screen and (max-width: 1140px) {
    .testamonial {
        width: 573px;
        height: 253px;

        .contain-text {
            .name-telltale {
                padding-top: 16px;
            }

            .profession-telltale {
                padding-bottom: 16px;
            }
        }
    }
}

@media screen and (max-width: 600px) {
    .testamonial {
        width: 327px;
        height: 278px;
    }
}

</style>
    
