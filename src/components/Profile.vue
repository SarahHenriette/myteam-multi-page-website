<template>
    <div class="director-profile general-profile">
        <div v-if="recto" class="contain-infos-profil">
            <div class="contain-profile-img">
            <img :src= img  alt="">
            </div>
            <p class="name-director name-director-general"> {{ name }} </p>
            <p class="profession-director"> {{ profession }} </p>
        </div>
        <div v-else class="contain-infos-profil">
              <p class="name-director">  {{ name }} </p>
              <p class="citation-director"> {{ citation }} </p>
              <div class="icon">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="20"><path fill="" d="M24 2.557a9.83 9.83 0 01-2.828.775A4.932 4.932 0 0023.337.608a9.864 9.864 0 01-3.127 1.195A4.916 4.916 0 0016.616.248c-3.179 0-5.515 2.966-4.797 6.045A13.978 13.978 0 011.671 1.149a4.93 4.93 0 001.523 6.574 4.903 4.903 0 01-2.229-.616c-.054 2.281 1.581 4.415 3.949 4.89a4.935 4.935 0 01-2.224.084 4.928 4.928 0 004.6 3.419A9.9 9.9 0 010 17.54a13.94 13.94 0 007.548 2.212c9.142 0 14.307-7.721 13.995-14.646A10.025 10.025 0 0024 2.557z"/></svg>
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20"><path fill="" d="M18 0H2C.9 0 0 .9 0 2v16c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V2c0-1.1-.9-2-2-2zM6 17H3V8h3v9zM4.5 6.3c-1 0-1.8-.8-1.8-1.8s.8-1.8 1.8-1.8 1.8.8 1.8 1.8-.8 1.8-1.8 1.8zM17 17h-3v-5.3c0-.8-.7-1.5-1.5-1.5s-1.5.7-1.5 1.5V17H8V8h3v1.2c.5-.8 1.6-1.4 2.5-1.4 1.9 0 3.5 1.6 3.5 3.5V17z"/></svg>
              </div>
          </div>
        <div :class="versoActive" class="btn-circle pink" @click="greet" > <img v-if="recto" src="images/icon-cross.svg"  alt=""> <svg v-else xmlns="http://www.w3.org/2000/svg" width="18" height="17"><path fill="" fill-rule="evenodd" d="M15.01.368l2.122 2.122-6.01 6.01 6.01 6.01-2.122 2.122L9 10.622l-6.01 6.01L.868 14.51 6.88 8.5.87 2.49 2.988.368 9 6.38 15.01.37z"/></svg></div>
    </div>
</template>

<script>
export default {
    props: ['img','name', 'profession', 'classBtn', 'imgBtnCircle', 'citation'],
    components: {
    },
    data: function (){
        return {
            recto: true,
            versoActive: "",
        }
    }, 
    methods: {
        greet: function (e){
            if(this.recto == true){
                this.recto = false
                this.versoActive = "active"
                e.target.parentNode.style.backgroundColor= "#002529"
            }else {
                this.recto = true
                this.versoActive = ""
            }
        }
    }
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
        .citation-director {
            font-style: normal;
            font-weight: 500;
            font-size: 15px;
            line-height: 25px;
            text-align: center;
            color: $white;
            padding-top: 8px;
            width: 250px;
            text-align: center;
        }
          .icon {
          width: 60px;
          height: 20px;
          margin: auto;
          display: flex;
          justify-content: space-between;
          margin-top: 24px;
          svg {
              fill: $white;
              cursor: pointer;
              transition: fill ease .5s;
              &:hover  {
                  fill: $lightCoral;
              }
          }
        }
    }
    .pink {
        background-color: $lightCoral;
        cursor: pointer;
        transition: background-color ease .2s;
        
        &:hover {
            background-color: $raptureBlue;
        }
        img {
            pointer-events: none;
        }
         svg {
              fill: $darkGreen;
              pointer-events: none;
            }
    }
    .active {
        background-color: $raptureBlue;
        cursor: pointer;
        transition: background-color ease .2s;
        &:hover {
            background-color: $lightCoral;
        }
    }
}
</style>