<template>
  <div class="about">
    <header class="header-about">
      <div class="text-header-about">
        <h1>About</h1>
        <p><span></span> We help companies build dynamic teams made up of top global talent.
          Using our network of passionate professionals we drive innovation
          and deliver incredible outcomes. Talented, diverse teams shape the
          best products and experiences. We’ll bring those teams to you.</p>
      </div>
      <svg xmlns="http://www.w3.org/2000/svg" width="200" height="200">
        <g fill="none" fill-rule="evenodd">
          <path fill="#2C6269" d="M100 100H0V0h100z" />
          <path fill="#F67E7E"
            d="M100 0c55.228 0 100 44.772 100 100s-44.772 100-100 100S0 155.228 0 100 44.772 0 100 0zm0 67c-18.225 0-33 14.775-33 33s14.775 33 33 33 33-14.775 33-33-14.775-33-33-33z" />
          <path fill="#79C8C7"
            d="M100 40v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0V8h100zm0-8v4H0V0h100z" />
        </g>
      </svg>
    </header>
  </div>
</template>

<script>
  export default {
    name: 'About',
    components: {}
  }
</script>

<style lang="scss" scoped>
  @import './public/sass/colors.scss';

  .header-about {
    background-color: $midnightGreen;
    width: 100%;
    height: 517px;
    position: relative;
    overflow: hidden;

    .text-header-about {
      width: 1110px;
      height: 156px;
      display: flex;
      margin: auto;
      padding-top: 241px;

      h1 {
        font-size: 64px;
        font-weight: bold;
        line-height: 100px;
        color: $white;
        width: 350px;
        margin-top: 0;
        margin-bottom: 0;
      }

      p {
        font-size: 18px;
        line-height: 28px;
        font-weight: 600;
        width: 730px;
        color: $white;
        display: flex;
        flex-direction: column;
        justify-content: space-between;

        span {
          width: 50px;
          height: 4px;
          background-color: $lightCoral;
        }
      }
    }

    svg {
      position: absolute;
      top: 317px;
      right: -100px;
    }

  }

  @media screen and (max-width: 1390px) {
    .header-about {
      width: 100%;

      .text-header-about {
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
        padding-top: 224px;

        h1 {
          text-align: center;
        }

        p {
          width: 457px;
          text-align: center;
          font-size: 15px;

          span {
            display: none;
          }
        }
      }
    }
  }

@media screen and (max-width: 690px) {
  .header-about {
    height: 520px;
    .text-header-about {
      padding-top: 160px;
      height: 252px;

      h1 {
        font-size: 40px;
        line-height: 40px;
        margin-bottom: 16px;
      }
      p {
        width: 327px;
      }
    }
    svg {
      top: 420px;
    }
  }
}
</style>