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
        img.bubble(src="~assets/bubble.png").is-hidden-mobile
  section
    .columns
      .column 
      .column
        .full-block.red Play Up Alps fédère et facilite l’organisation d’événements startup dans l’arc Alpin
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
      .more-info
        h3 en savoir plus 
  section
    .container
      h3.number-tag #2
      .bloc#sw
        h4.section-title Les Startup Weekend
        .blue-text
          h4 De l'idée à la startup
          p  Le Startup Weekend est un événement dont le concept a été initié aux Etats-Unis en 2007 à Boudler, Colorado. Il est porté par Techstars de Google for Entrepreneurs.
  section
    .container
      .blue-section
        p Ces événements permettent de révéler le dynamisme de l’écosystème entrepreneurial local au travers de 54 heures de travail collaboratif. Chaque année, une startup est distinguée, et de nombreux projets sont mis sur les rails grâce à un accompagnement stratégique sur-mesure.
        p.light En plus de 10 ans, il s’est exporté partout dans le monde, notamment en France. On compte plus de 4000 éditions dans près de 1200 villes et 140 pays, rassemblant plus de 230 000 participants !
  section
    .columns
      .column 
      .column
        .full-block.white Découvrez dès à present nos éditions alpines
  section
    .container
      h3.number-tag #3
      .bloc
        .association
          h4.section-title Prochains rendez-vous
    .container-fluid
      .bg-block
        .bg-blue  
        .bg-grey
      .container
        .columns
          .column.is-8.is-offset-2
            eventCard(:img-url="'https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_200/v1538901367/PlayUpApls/logo-annecy.png'", city="Annecy", place="Les Papeteries", address="1 Esplanade Augustin Aussedat", text="à partir de 18h", date="12-14", month="octobre", link-url="http://www.startupweekendannecy.com/")
            eventCard(:img-url="'https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_200/v1538901367/PlayUpApls/logo-grenoble.png'", city="Grenoble", place="IAE Grenoble", address="525 Avenue Centrale 38400 Saint-Martin-d'Hères", text="à partir de 18h", date="16-18", month="novembre", link-url="http://www.swgrenoble.org/")
            eventCard(:img-url="'https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_200/v1538901367/PlayUpApls/logo-chambery.png'", city="Chambéry", place="Le Manége", address="1 Esplanade Augustin Aussedat", text="à partir de 18h", date="1-3", month="février", link-url="#")
  section
    .container
      h3.number-tag #4
      .bloc
        .association
          h4.section-title Nos sponsors
    .container-fluid
      .columns.sponsors
        .column
        .column.has-text-centered
          a(href="https://my-mg.com/")
            img(src="https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_100/v1538908951/PlayUpApls/mg.png")
        .column.has-text-centered
          a(href="http://pandorabox-consulting.com/")
            img(src="https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_100/v1538909245/PlayUpApls/pandorabox.png")
        .column

        

</template>

<script>
import eventCard from "../components/eventCard.vue";
export default {
  components: { eventCard }
};
</script>

<style lang="stylus">
.bg-block {
  margin-top: 60px;
  z-index: -1;
  position: relative;

  .bg-blue {
    position: absolute;
    background-color: #1F2951;
    width: 100%;
    height: 100px;
    transform-origin: center;
    transform: rotate(-8deg) translateX(-100px);
  }

  .bg-grey {
    top: 100px;
    position: absolute;
    background-color: #F2F2F2;
    width: 100%;
    height: 780px;
    transform-origin: center;
    transform: rotate(-5deg) translateY(-60px);
  }
}

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

.full-block {
  font-size: 18px;
  line-height: 28px;
  padding: 30px 0 30px 30px;
}

.red {
  background-color: #E4003A;
  color: #FFFFFF;
}

.white {
  transform: translateY(-50px);
  background-color: #FFFF;
}

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

.blue-section {
  background-color: #1F2951;
  font-size: 18px;
  color: #FFFFFF;
  line-height: 28px;
  padding: 46px;

  p.light {
    /* En plus de 10 ans, i: */
    font-family: Montserrat-Regular;
    font-size: 13px;
    color: #FFFFFF;
    line-height: 23px;
    margin: 30px 0;
  }
}

.more-info {
  :before {
    content: url('/assets/micro-logo.svg');
    margin-right: 10px;
  }

  margin-top: 20px;
  padding-right: 20px;
  background-color: #E4003A;
  text-align: right;
  color: #FFFF;
  text-transform: uppercase;
}

#sw {
  display: flex;
  justify-content: space-between;
}

.blue-text {
  width: 40%;
  margin-bottom: 50px;

  h4 {
    font-family: Montserrat-Regular;
    font-size: 27px;
    color: #FFFFFF;
    letter-spacing: 0.64px;
    line-height: 25px;
    background-color: #1F2951;
    margin-bottom: 15px;
  }

  p {
    text-align: justify;
    font-family: Montserrat-Regular;
    font-size: 13px;
    color: #000000;
    line-height: 20px;
  }
}

.sponsors {
  margin-top: 50px;
}
</style>

