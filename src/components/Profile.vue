<template>
    <div class="director-profile general-profile">
        <div class="contain-infos-profil">
            <div class="contain-profile-img">
            <img :src= img  alt="">
            </div>
            <p class="name-director name-director-general"> {{ name }} </p>
            <p class="profession-director"> {{ profession }} </p>
        </div>
        <div class="btn-circle pink"> <img src="images/icon-cross.svg"  alt=""> </div>
    </div>
</template>

<script>
export default {
    props: ['img','name', 'profession', 'classBtn', 'imgBtnCircle']
}
</script>

<style lang="scss" scoped>
    @import './public/sass/colors.scss';
    @import './public/sass/profile.scss';

.general-profile {
    background-color: $sacramentoStateGreen;

    .contain-infos-profil {
        .contain-profile-img {
            width: 96px;
            height: 96px;
            border: 2px solid #C4FFFE;
            border-radius: 50%;
            overflow: hidden;
            margin: auto;

            img {
                width: 100%;
            }
        }

        .name-director-general {
            padding-top: 16px;
        }

        .profession-director {
            font-style: italic;
            font-weight: 500;
            font-size: 15px;
            line-height: 25px;
            text-align: center;
            color: $white;
        }
    }

    .pink {
        background-color: $lightCoral;
    }

}
</style>