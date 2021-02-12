<template>
  <div class="home">
    <Header />
    <section class="keyPoints">
      <div class="contain-text">
        <h2><span></span> Build & manage distributed teams like no one else.</h2>
        <div class="container-keysPoints">
          <KeyPoint img="images/icon-person.svg" alt="jolie icon d'un individus" title="Experienced Individuals"
            text="Our network is made up of highly experienced professionals who are passionate about what they do." />
          <KeyPoint img="images/icon-cog.svg" alt="roue de parametre valide" title="Enhanced Productivity"
            text="Our processes have been refined over years of implementation meaning our teams always deliver." />
          <KeyPoint img="images/icon-chart.svg" alt="joli design de graphique" title="Enhanced Productivity"
            text="Our customized platform with in-built analytics helps you manage your distributed teams." />
        </div>
      </div>
      <svg xmlns="http://www.w3.org/2000/svg" class="image-background" width="200" height="244">
        <g fill="none" fill-rule="evenodd">
          <path fill="#2C6269" d="M100 144H0V44h100z" />
          <path fill="#014E56"
            d="M100 44c55.228 0 100 44.772 100 100s-44.772 100-100 100S0 199.228 0 144 44.772 44 100 44zm0 67c-18.225 0-33 14.775-33 33s14.775 33 33 33 33-14.775 33-33-14.775-33-33-33z" />
          <path fill="#79C8C7"
            d="M100 184v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zm0-8v4H0v-4h100zM4 40v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zM4 32v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zM4 24v4H0v-4h4zm7 0v4H7v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm7 0v4h-4v-4h4zm-35-8v4h-4v-4h4zm14 0v4h-4v-4h4zm-7 0v4h-4v-4h4zm21 0v4h-4v-4h4zm-7 0v4h-4v-4h4zM4 16v4H0v-4h4zm7 0v4H7v-4h4zm42 0v4h-4v-4h4zM4 8v4H0V8h4zm7 0v4H7V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zm7 0v4h-4V8h4zM4 0v4H0V0h4zm7 0v4H7V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4zm7 0v4h-4V0h4z" />
        </g>
      </svg>
    </section>
    <section class="testamonials">
      <div class="contain-text">
          <h2>Delivering real results for top companies. Some of our <span>success stories.</span></h2>
          <div class="contain-testamonials">
                <Testamonial text=" “The team perfectly fit the specialized skill set required. They focused on the most essential features helping us launch the platform eight months faster than planned.”" 
                      name="Kady Baker" profession="Product Manager at Bookmark" img="images/avatar-kady.jpg" alt="kady, portrait d'une femme blonde et souriante"/>

                <Testamonial text="“We needed to automate our entire onboarding process. The team came in and built out the whole journey. Since going live, user retention has gone through the roof!”"
                              name="Aiysha Reese" profession="Founder of Manage" img="images/avatar-aiysha.jpg" alt="aiysha, très belle femme entrepreneuse"/>

                <Testamonial text="“Amazing. Our team helped us build an app that delivered a new experience for hiring a physio. The launch was an instant success with 100k downloads in the first month.”" 
                              name="Arthur Clarke" profession="Co-founder of MyPhysio" img="images/avatar-arthur.jpg" alt="arthur, homme fort et expérimenté"/>         
          </div>  
          <svg xmlns="http://www.w3.org/2000/svg" class="image-background-top" width="147" height="100"><g fill="none" fill-rule="evenodd"><path fill="#002529" d="M0 100h100V0H0z"/><path fill="#79C8C7" d="M47 96v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47zm0-8v4h100v-4H47z"/></g></svg>         
          <svg xmlns="http://www.w3.org/2000/svg" class="image-background-bottom" width="200" height="100"><g fill="none" fill-rule="evenodd"><path fill="#2C6269" d="M100 100h100V0H100z"/><path fill="#012F34" d="M100 0C44.772 0 0 44.772 0 100s44.772 100 100 100 100-44.772 100-100S155.228 0 100 0zm0 67c18.225 0 33 14.775 33 33s-14.775 33-33 33-33-14.775-33-33 14.775-33 33-33z"/><path fill="#79C8C7" d="M100 96v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100zm0-8v4h100v-4H100z"/></g></svg>
      </div>
    </section>
    <ContactUs/>
    <Footer/>
  </div>
</template>

<script>
import Header from './../components/HeaderHome'
import KeyPoint from './../components/KeyPoints'
import Testamonial from './../components/Testamonial'
import ContactUs from './../components/ContactUs'
import Footer from './../components/Footer'

export default {
  name: 'Home',
  components: {
    Header,
    KeyPoint,
    Testamonial,
    ContactUs,
    Footer
  },
  data: function() {
    return {
      message: '',
    }
  }
}
</script>

<style lang="scss" scoped>
  @import './public/sass/colors.scss';
  .keyPoints {
    background-color: $sacramentoStateGreen;
    width: 100%;
    height: 684px;
    display: flex;
    margin: auto;
    position: relative;
    overflow: hidden;

    h2 {
      margin: 0;
      width: 445px;
      height: 202px;
      font-size: 48px;
      line-height: 48px;
      font-weight: 700;
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

    .contain-text {
      display: flex;
      margin: auto;
      width: 1110px;
      height: 404px;
      justify-content: space-between;

      .container-keysPoints {
        width: 540px;
        height: 346px;
        margin-top: 58px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
      }
    }

    .image-background {
      position: absolute;
      right: -100px;
      bottom: 0;
    }
  }

  @media screen and (max-width: 1220px) {
    .keyPoints {
      flex-direction: column;
      height: 710px;

      h2 {
        margin-left: 0;
        width: 445px;
        height: 100px;
        font-size: 32px;
        line-height: 32px;
      }

      .contain-text {
        width: 573px;
        height: 510px;
        flex-direction: column;

        .container-keysPoints {
          margin-top: 64px;
          margin-left: 0;
        }
      }

    }

    .image-background {
      top: 0;
    }
  }

  @media screen and (max-width: 690px) {
    .keyPoints {
      height: 1073px;

      h2 {
        width: 207px;
        height: 196px;
      }

      .contain-text {
        width: 327px;
        height: 945px;

        .container-keysPoints {
          margin-top: 56px;
          width: 327px;
          height: 693px;
        }
      }

    }
  }

.testamonials {
  width: 100%;
  height: 745px;
  background-color: $midnightGreen;
  position: relative;

  h2 {
    width: 932px;
    height: 96px;
    font-style: normal;
    font-weight: bold;
    font-size: 48px;
    line-height: 48px;
    text-align: center;
    color: $white;
    margin: auto;
    padding-top: 140px;
    padding-bottom: 56px;

    span {
      color: $raptureBlue;
    }
  }

  .contain-testamonials {
    display: flex;
    justify-content: space-between;
    width: 1110px;
    height: 313px;
    margin: auto;
  }

  .image-background-top {
    position: absolute;
    top: 0;
    left: 0;
  }

  .image-background-bottom {
    position: absolute;
    bottom: 0;
    right: 0;
  }
}

@media screen and (max-width: 1140px) {
  .testamonials {
    height: 1199px;

    h2 {
      width: 485px;
      height: 96px;
      font-size: 32px;
      line-height: 32px;
      padding-top: 100px;
      padding-bottom: 48px;
    }

    .contain-testamonials {
      flex-direction: column;
      height: 855px;
      width: 573px;
    }
  }
}

@media screen and (max-width: 600px) {
  .testamonials {
    height: 1410px;

    h2 {
      width: 327px;
      height: 128px;
      padding-top: 140px;
    }

    .contain-testamonials {
      width: 327px;
      height: 930px;
    }
  }
}
</style>
