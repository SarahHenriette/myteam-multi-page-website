<template>
  <div class="about">
    <Header/>
    <section class="directors">
      <h2>Meet the directors</h2>
      <div class="container-directors">
        <Profile img = "images/avatar-nikita.jpg" alt="nikita, une jeune femme brune et souriante" name ="Nikita Marks" profession ="Founder & CEO" classBtn="btn-circle pink"/>
        <Profile img = "images/avatar-christian.jpg" alt="christian, un jeune homme souriant et dynamique" name ="Christian Duncan" profession ="Co-founder & COO"/>
        <Profile img = "images/avatar-cruz.jpg" alt="cruz, un homme souriant et competant" name ="Cruz Hamer" profession ="Co-founder & CTO"/>
        <Profile img = "images/avatar-drake.jpg" alt="drake, un homme sérieux et travailleur" name ="Drake Heaton" profession ="Business Development Lead"/>
        <Profile img = "images/avatar-griffin.jpg" alt="griffin, jeune homme très compétent" name ="Griffin Wise" profession ="Lead Marketing"/>
        <ProfileReverse name="Aden Allan" alt="allan, jeune hommme competent" citation="“Empowered teams create truly amazing products. Set the north star and let them follow it.”"/>
      </div>
      <svg xmlns="http://www.w3.org/2000/svg" class="img-background-top" width="200" height="200"><g fill="none" fill-rule="evenodd"><path fill="#2C6269" d="M100 100h100V0H100z"/><path fill="#012F34" d="M100 0C44.772 0 0 44.772 0 100s44.772 100 100 100 100-44.772 100-100S155.228 0 100 0zm0 67c18.225 0 33 14.775 33 33s-14.775 33-33 33-33-14.775-33-33 14.775-33 33-33z"/><path fill="#79C8C7" d="M100 96v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100z"/><path fill="#F67E7E" d="M196 140v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm35-8v4h4v-4h-4zm-14 0v4h4v-4h-4zm7 0v4h4v-4h-4zm-21 0v4h4v-4h-4zm7 0v4h4v-4h-4zm35 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-42 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4z"/></g></svg>
      <svg xmlns="http://www.w3.org/2000/svg" class="img-background-bottom" width="147" height="100"><g fill="none" fill-rule="evenodd"><path fill="#002529" d="M0 100h100V0H0z"/><path fill="#79C8C7" d="M47 96v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47z"/></g></svg>
    </section>
  </div>
</template>

<script>
  // @ is an alias to /src
  import Header from "./../components/HeaderAbout"
  import Profile from "./../components/Profile"
  import ProfileReverse from  "./../components/ProfileReverse"

  export default {
    name: 'About',
    components: {
      Header,
      Profile,
      ProfileReverse
    }
  }
</script>

<style lang="scss" scoped>
@import './public/sass/colors.scss';

.directors {
  width: 100%;
  height: 1002px;
  background-color: $deepJungleGreen;
  margin-top: -1px;
  position: relative;
  overflow: hidden;
  h2 {
    margin: 0;
    font-style: normal;
    font-weight: bold;
    font-size: 48px;
    line-height: 48px;
    text-align: center;
    color: $white;
    padding-top: 140px;
  }
  .container-directors {
    width: 1110px;
    height: 610px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    padding-top: 64px;
  }
  .img-background-top {
    position: absolute;
    top: 0;
    left: -100px;
  }
  .img-background-bottom {
    position: absolute;
    bottom: 0;
    right: 0;
  }
}

@media screen and (max-width: 1120px) {
  .directors {
    height: 1219px;
    h2 {
      font-size: 32px;
      line-height: 32px;
      padding-top: 100px;
    }
     .container-directors {
       width: 573px;
       height: 939px;
       padding-top: 48px;
     }
  }
}

@media screen and (max-width: 600px) {
  .directors {
    height: 2062px;
    h2 {
      padding-top: 88px;
    }
    .container-directors {
      width: 327px;
      height: 1806px;
    }
    .img-background-top {
      top: -100px;
    }
  }
}

</style>