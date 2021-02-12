<template>
  <div class="home">
    <header class="header-home">
      <div class="text-header-home">
        <h1>Find the<br/> best <span>talent</span></h1>
        <p><span></span> Finding the right people and building high performing teams can 
        be hard. Most companies aren’t tapping into the abundance of global 
        talent. We’re about to change that.</p>
      </div>
      <svg xmlns="http://www.w3.org/2000/svg" class="img-background-dark" width="200" height="200"><g fill="none" fill-rule="evenodd"><path fill="#79C8C7" d="M100 200h100V100H100z"/><path fill="#012F34" d="M100 0C44.772 0 0 44.772 0 100s44.772 100 100 100 100-44.772 100-100S155.228 0 100 0zm0 67c18.225 0 33 14.775 33 33s-14.775 33-33 33-33-14.775-33-33 14.775-33 33-33z"/><path fill="#F67E7E" d="M196 196v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm35-8v4h4v-4h-4zm-14 0v4h4v-4h-4zm7 0v4h4v-4h-4zm-21 0v4h4v-4h-4zm7 0v4h4v-4h-4zm35 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-42 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4z"/></g></svg>
      <svg xmlns="http://www.w3.org/2000/svg" class="img-background-pink" width="358" height="100"><g fill="none" fill-rule="evenodd"><circle cx="100" cy="100" r="100" fill="#2C6269"/><path fill="#012F34" d="M258 0c55.228 0 100 44.772 100 100s-44.772 100-100 100-100-44.772-100-100S202.772 0 258 0zm0 67c-18.225 0-33 14.775-33 33s14.775 33 33 33 33-14.775 33-33-14.775-33-33-33z"/><path fill="#79C8C7" d="M358 43h-43V0h43z"/><path fill="#F67E7E" d="M233.514 0c55.228 0 100 44.772 100 100s-44.772 100-100 100c-55.229 0-100-44.772-100-100s44.771-100 100-100zm0 67c-18.226 0-33 14.775-33 33s14.774 33 33 33c18.225 0 33-14.775 33-33s-14.775-33-33-33z"/><path fill="#79C8C7" d="M100 40v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0V8h100zm0-8v4H0V0h100z"/></g></svg>
    </header>
  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'Home',
  components: {
  }
}
</script>

<style lang="scss" scoped>
@import './public/sass/colors.scss';

.header-home {
  background-color: $midnightGreen;
  width: 100%;
  height: 700px;
  position: relative;

  .text-header-home {
    width: 1110px;
    height: 200px;
    display: flex;
    margin: auto;
    padding-top: 250px;

    h1 {
      font-size: 100px;
      font-weight: 700;
      line-height: 100px;
      color: $white;
      width: 635px;
      margin-top: 0;
      margin-bottom: 0;

      span {
        color: $lightCoral;
      }
    }

    p {
      font-size: 18px;
      line-height: 28px;
      font-weight: 600;
      width: 445px;
      color: $white;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      padding-left: 30px;  
      span {
        width: 50px;
        height: 4px;
        background-color: $raptureBlue;
      }
    }
  }

  .img-background-dark {
    position: absolute;
    top: 250px;
    left: -100px;
  }

  .img-background-pink {
    position: absolute;
    top: 600px;
    left: 917px;
  }
}

@media screen and (max-width: 1390px) {
  .header-home {
    width: 100%;

    .text-header-home {
      width: 683px;
      flex-direction: column;
      align-items: center;

      h1 {
        font-size: 64px;
        line-height: 56px;
        text-align: center;
        width: 100%;
        margin-bottom: 24px;
      }

      p {
        text-align: center;
        font-size: 15px;
        width: 505px;

        span {
          display: none;
        }
      }
    }

    .img-background-dark {
      display: none;
    }

    .img-background-pink {
      position: absolute;
      top: 600px;
      left: 0;
      right: 0;
      margin: auto;
    }
  }
}

@media screen and (max-width: 690px) {
  .header-home {
    height: 567px;

    .text-header-home {
      width: 327px;
      padding-top: 160px;

      h1 {
        font-size: 40px;
        line-height: 40px;
      }

      p {
        width: 336px;
      }
    }

    .img-background-pink {
      top: 467px;
    }
  }
}
</style>
