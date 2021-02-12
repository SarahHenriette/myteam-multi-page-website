<template>
    <div class="keyPoint">
        <img :src= img :alt= alt>
        <div class="text-keyPoint">
            <h4> {{ title }}</h4>
            <p> {{ text }} </p>
        </div>
    </div>
</template>

<script>
export default {
    props: ["img", "alt", "title", "text"]
}
</script>

<style lang="scss" scoped>
  @import './public/sass/colors.scss';
.keyPoint {
    display: flex;
    align-items: flex-start;
    width: 540px;
    height: 94px;

    .text-keyPoint {
        width: 445px;
        margin-left: 23px;

        h4 {
            color: $lightCoral;
            margin-top: 0;
            margin-bottom: 16px;
            font-size: 18px;
            font-weight: 700;
        }

        p {
            font-size: 15px;
            color: $white;
            line-height: 25px;
            width: 430px;
        }
    }
}

@media screen and (max-width: 1210px) {
    .keyPoint .text-keyPoint {
        p {
            width: 100%;

        }
    }
}

@media screen and (max-width: 690px) {
    .keyPoint {
        width: 327px;
        height: 199px;
        flex-direction: column;

        .text-keyPoint {
            width: 327px;
            height: 111px;
            text-align: center;
            margin-left: 0;

            h4 {
                font-size: 18px;
                line-height: 28px;
                margin-top: 16px;
                margin-bottom: 8px;
            }
        }
    }
}
</style>