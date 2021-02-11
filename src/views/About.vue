<template>
  <div class="about">
    <Header/>
    <section class="directors">
      <h2>Meet the directors</h2>
      <div class="container-directors">
        <Profile img = "images/avatar-nikita.jpg" alt="nikita, une jeune femme brune et souriante" name ="Nikita Marks" profession ="Founder & CEO" classBtn="btn-circle pink" citation="“Empowered teams create truly amazing products. Set the north star and let them follow it.”"/>
        <Profile img = "images/avatar-christian.jpg" alt="christian, un jeune homme souriant et dynamique" name ="Christian Duncan" profession ="Co-founder & COO" citation="“Empowered teams create truly amazing products. Set the north star and let them follow it.”"/>
        <Profile img = "images/avatar-cruz.jpg" alt="cruz, un homme souriant et competant" name ="Cruz Hamer" profession ="Co-founder & CTO" citation="“Empowered teams create truly amazing products. Set the north star and let them follow it.”"/>
        <Profile img = "images/avatar-drake.jpg" alt="drake, un homme sérieux et travailleur" name ="Drake Heaton" profession ="Business Development Lead" citation="“Empowered teams create truly amazing products. Set the north star and let them follow it.”"/>
        <Profile img = "images/avatar-griffin.jpg" alt="griffin, jeune homme très compétent" name ="Griffin Wise" profession ="Lead Marketing" citation="“Empowered teams create truly amazing products. Set the north star and let them follow it.”"/>
        <Profile img = "images/avatar-aden.jpg" alt="aden, jeune homme très fun et travailleur" name ="Aden Allen" profession = "Head of talent" citation="“Empowered teams create truly amazing products. Set the north star and let them follow it.”"/>
        
        <!-- <ProfileReverse name="Aden Allan" alt="allan, jeune hommme competent" citation="“Empowered teams create truly amazing products. Set the north star and let them follow it.”"/> -->
      </div>
      <svg xmlns="http://www.w3.org/2000/svg" class="img-background-top" width="200" height="200"><g fill="none" fill-rule="evenodd"><path fill="#2C6269" d="M100 100h100V0H100z"/><path fill="#012F34" d="M100 0C44.772 0 0 44.772 0 100s44.772 100 100 100 100-44.772 100-100S155.228 0 100 0zm0 67c18.225 0 33 14.775 33 33s-14.775 33-33 33-33-14.775-33-33 14.775-33 33-33z"/><path fill="#79C8C7" d="M100 96v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100z"/><path fill="#F67E7E" d="M196 140v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm35-8v4h4v-4h-4zm-14 0v4h4v-4h-4zm7 0v4h4v-4h-4zm-21 0v4h4v-4h-4zm7 0v4h4v-4h-4zm35 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-42 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm49-8v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4zm-7 0v4h4v-4h-4z"/></g></svg>
      <svg xmlns="http://www.w3.org/2000/svg" class="img-background-bottom" width="147" height="100"><g fill="none" fill-rule="evenodd"><path fill="#002529" d="M0 100h100V0H0z"/><path fill="#79C8C7" d="M47 96v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47z"/></g></svg>
    </section>
    <section class="clients">
      <h2>Some of our clients</h2>
      <div class="contain-logo-clients">
        <div class="contain-logo logo-verge">
          <img src="images/logo-the-verge.png" alt="logo de the verge">
        </div>
        <div class="contain-logo logo-jakarta">
          <img src="images/logo-jakarta-post.png" alt="logo de jakarta post">
        </div>
        <div class="contain-logo logo-guardian">
          <img src="images/logo-the-guardian.png" alt="logo de the guadian">
        </div>
        <div class="contain-logo logo-tech">
          <img src="images/logo-tech-radar.png" alt="logo de tech radar">
        </div>
        <div class="contain-logo logo-gadget">
          <img src="images/logo-gadgets-now.png" alt="logo de gadgets now">
        </div>
      </div>
      <svg xmlns="http://www.w3.org/2000/svg" width="200" height="200"><g fill="none" fill-rule="evenodd"><path fill="#2C6269" d="M100 100H0V0h100z"/><path fill="#014E56" d="M100 0c55.228 0 100 44.772 100 100s-44.772 100-100 100S0 155.228 0 100 44.772 0 100 0zm0 67c-18.225 0-33 14.775-33 33s14.775 33 33 33 33-14.775 33-33-14.775-33-33-33z"/><path fill="#79C8C7" d="M100 140v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zM4 40v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zM4 32v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zM4 24v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm-35-8v4h-4v-4h4zm14 0v4h-4v-4h4zm-7 0v4h-4v-4h4zm21 0v4h-4v-4h4zm-7 0v4h-4v-4h4zM4 16v4H0v-4h4zm7 0v4H7v-4h4zm42 0v4h-4v-4h4zM4 8v4H0V8h4zm7 0v4H7V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zM4 0v4H0V0h4zm7 0v4H7V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4z"/></g></svg>
    </section>
    <ContactUs/>
    <Footer/>
  </div>
</template>

<script>
  // @ is an alias to /src
  import Header from "./../components/HeaderAbout"
  import Profile from "./../components/Profile"
  // import ProfileReverse from  "./../components/ProfileReverse"
  import ContactUs from './../components/ContactUs'
  import Footer from './../components/Footer'
  export default {
    name: 'About',
    components: {
      Header,
      Profile,
      // ProfileReverse,
      ContactUs,
      Footer
    }, 
    // data (){
    //   return {
    //     test: true,      
          
    //   }
     
    // },
    //    methods: {
    //     test2: function (){

    //     }
    // }
    
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

.clients {
  width: 100%;
  height: 437px;
  background-color: $darkGreen;
  position: relative;
  overflow: hidden;
  margin: -1px;
  h2 {
    width: 920px;
    height: 48px;
    font-style: normal;
    font-weight: bold;
    font-size: 48px;
    line-height: 48px;
    text-align: center;
    color: $white;
    
    margin: auto;
    padding-top: 140px;
  }
  .contain-logo-clients {
    width: 1110px;
    height: 45px;
    display: flex;
    justify-content: space-between;
    margin: auto;
    margin-top: 64px;
       .contain-logo {
            width: 180px;
        height: 100px;
        img {
        max-width: 100%;
        height: auto;
      }
      }
        .logo-gadget {
        height: 100%;
        width: auto;
        img {
          height: 100%;
        }
      }
      .logo-verge {
            width: 165px;
      }
      .logo-jakarta {
            width: 184px;

      }
      .logo-tech {
            width: 165px;

      }
  }
  svg {
    position: absolute;
    top: 0;
    left: 0;
  }
}

@media screen and (max-width: 1220px)  {
  .clients {
    height: 308px;
    h2 {
      font-size: 32px;
      line-height: 32px;
      padding-top: 100px;
      width: 457px;
      height: 32px;
    }
    .contain-logo-clients {
      width: 689px;
      margin-top: 48px;
      height: 28px;
      img {
        height: 17px;
      }
      .contain-logo {
            width: 122px;

      }
      .logo-gadget {
        width: auto;
      }
            .logo-verge {
            width: 103px;
      }
      .logo-jakarta {
            width: 114px;

      }
      .logo-guardian {
        width: 112px;
      }
      .logo-tech {
            width: 103px;

      }
    }
    svg {
      top: -100px;
    }
  }
}
@media screen and (max-width: 600px)  {
  .clients {
    height: 632px;
    h2 {
      width: 327px;
    }
    .contain-logo-clients {
      flex-direction: column;
          align-items: center;

      width: 162px;
      height: 360px;
      margin-top: 64px;
   .logo-gadget {
            width: 87px;
            height: auto;
          img {
            height: auto;
          }
      }
      .logo-verge {
      width: 146px;
      }
      .logo-jakarta {
            width: 162px;

      }
      .logo-guardian {
        width: 159px;
      }
      .logo-tech {
            width: 146px;

      }
    }
    svg {
      left: -100px;
    }
  }
}
</style>