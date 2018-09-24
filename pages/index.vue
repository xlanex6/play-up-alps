<template lang="pug">
div
  section.has-bg-img
    .container
      .header
        .pua-navbar
          img.logo(src="~assets/logo.png")
        .pua-header
          .red-block 
            | Activer et rassembler l’arc alpin pour 
            br 
            |contribuer au développement de réussites
          .white-block Organisateur des Startup Weekend
          .logo
            img(src="~assets/logo-title.png")
        img.bubble(src="~assets/bubble.png")
  section
    .columns
      .column 
      .column
        .full-red-block Play Up Alps fédère et facilite l’organisation d’événements startup dans l’arc Alpin
  section
    .container
      h3.number-tag #1
      .bloc
        .association
          h4.section-title L'association
          .white-bloc
            p Nous sommes un collectif bénévole avec un but commun :
            p.quote  «  Faire vivre une expérience différente et grandissante. »
          img(src="~assets/gre-pano.jpg")
  section
    .container
      h3.number-tag #2
      .bloc
        h4.section-title Les Startup Weekend


        //- .pua-highlight Activer et rassembler l’arc alpin pour contribuer au développement de réussites
</template>

<script>
import AppLogo from "~/components/AppLogo.vue";

export default {
  components: {
    AppLogo
  }
};
</script>

<style lang="stylus">
.pua-highlight {
  background: $primary;
  color: $white;
  letter-spacing: 0.64px;
  line-height: 25px;
}

.header {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.pua-navbar {
  img.logo {
    height: 35px;
    width: 50px;
    margin-top: 30px;
  }
}

.pua-header {
  margin-top: 100px;
  width: 60%;
  flex-direction: column;
  z-index: 1;

  .logo {
    margin-top: 60px;
  }
}

img.bubble {
  position: absolute;
  width: 632px;
  height: 507px;
  left: 35%; // bottom: 0;
  top: 30%;
  z-index: 0;

  // right: 0;

  // transform: translateX(36%);

  // top: 150px;
  // right: -37px;
  img {
    width: 100px;
  }
}

.has-bg-img {
  height: 640px;
  background: url('/assets/header-bg.jpg') center center;
  background-size: cover;
  position: relative;
}

h3.number-tag {
  font-size: 45px;
  color: #E4003A;
  letter-spacing: 0.6px;
}

.full-red-block {
  background-color: #E4003A;
  font-size: 18px;
  color: #FFFFFF;
  line-height: 28px;
  padding: 30px 0 30px 30px;
}

// h3:after {
// content: ' ';
// position: absolute;
// border-bottom: 2px solid #DAD8D8;
// }

// h3:before {
// content: ' ';
// position: absolute;
// border-bottom: 2px solid #DAD8D8;
// }

// h3:nth-of-type(1):before {
// width: 20%;
// height: 4px;
// margin: 7% 0 0 -7%;
// transform: rotate(-45deg);
// }

// h3:nth-of-type(1):after {
// width: 15%;
// height: 4px;
// margin: 9% 0 0 -9%;
// transform: rotate(-45deg);
// }
h4.section-title {
  font-size: 35px;
  color: #1F2951;
}

p.quote {
  font-size: 24px;
  color: #1F2951;
  line-height: 28px;
}

.bloc {
  padding-left: 60px;
  position: relative;
  // display: flex;
  // justify-content: center;
}

.association {
  .white-bloc {
    padding: 0 70px 27px 0;
    background: white;
    position: absolute;
  }
}

.red-block {
  font-size: 27px;
  letter-spacing: 0.64px;
  line-height: 25px;
  background-color: #E4003A;
  color: white;
}

.white-block {
  /* Rectangle 2: */
  background: #FFFFFF;
  width: 70%;
  /* Organisateur des Sta: */
  font-family: Montserrat-Regular;
  font-size: 20px;
  color: #1F2951;
  letter-spacing: 1px;
  line-height: 25px;
  margin-top: 10px;
}
</style>

