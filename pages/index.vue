<template lang="pug">
div
  section.has-bg-img
    .container
      .header
        .pua-navbar
          img.logo(src="~assets/logo.png")
        .pua-header
          .red-block 
            h3 Activer et rassembler l’arc alpin pour 
             br 
             |contribuer au développement de réussites
          .white-block Organisateur des Startup Weekend
          .logo
            img(src="~assets/logo-title.png")
        img.bubble(src="~assets/bubble.png").is-hidden-touch
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
          .columns
            .column
                p Nous sommes un collectif bénévole avec un but commun :
                p.quote  «  Faire vivre une expérience différente et grandissante. »
          .columns
            .column.has-text-centered
              img(src="~assets/gre-pano.jpg")
  section.is-hidden-touch
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
      .bg-block.is-hidden-touch
        .bg-blue  
        .bg-grey
      .container
        .columns
          .column.is-8.is-offset-2
            eventCard( :data-event="bigevent" )
            eventCard( :data-event="annecy" )
            eventCard(:data-event="grenoble")
            // eventCard( :data-event="chambery")
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
          a(href="https://my-mg.com/" target="_blank")
            img(src="https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_100/v1538908951/PlayUpApls/mg.png")
        .column.has-text-centered
          a(href="http://pandorabox-consulting.com/" target="_blank")
            img(src="https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_100/v1538909245/PlayUpApls/pandorabox.png")
        .column.has-text-centered
          a(href="https://levillagebyca.com/fr" target="_blank")
            img(src="https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_100/v1538909245/PlayUpApls/village-by-ca.png")
        .column
  section#footer
    .container-fluid
      .blue-section
        .container
          .columns
            .column.has-text-left.footer-text
              | Play Up Alps ® 2018
            .column
            .column.has-text-centered
              img.logo(src="~assets/logo.png")
              img(src="~assets/logo-title.png")
            .column
            .column.footer-text.footer-right
              a(href="mailto:hello@playupalps.com?subject=Depuis%20le%20site%20internet") 
                i.far.fa-envelope
        



</template>

<script>
import eventCard from "../components/eventCard.vue";
export default {
  components: { eventCard },
  data() {
    return {
      annecy: {
        imgUrl:
          "https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_200/v1538901367/PlayUpApls/logo-annecy.png",
        city: "Annecy",
        place: "Papeterie Image Factory",
        address: "1,3 Esplanade Augustin Aussedat, 74960",
        text: "à partir de 18h",
        date: "11-13",
        month: "octobre",
        linkUrl: "http://www.startupweekendannecy.com/"
      },
      grenoble: {
        imgUrl:
          "https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_200/v1538901367/PlayUpApls/logo-grenoble.png",
        city: "Grenoble",
        place: null,
        address: null,
        text: "à partir de 18h",
        date: "Mois de",
        month: "novembre",
        linkUrl: "http://www.swgrenoble.org/"
      },
      chambery: {
        imgUrl:
          "https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_200/v1538901367/PlayUpApls/logo-chambery.png",
        city: "Chambéry",
        place: "Le Manége",
        address: "331 Rue de la République",
        text: "à partir de 18h",
        date: "1-3",
        month: "février 20",
        linkUrl: "https://www.startupweekendchambery.com/"
      },
      bigevent: {
        imgUrl:
          "https://res.cloudinary.com/dey128wj1/image/upload/c_scale,h_200/v1555486065/PlayUpApls/logoBE.png",
        city: "Chambéry",
        place: "Place INEDIT",
        address: "Secret",
        text: "à partir de 18h",
        date: "23",
        month: "Mai",
        linkUrl: "/bigevent"
      }
    };
  }
};
</script>

<style lang="stylus">
body
  font-family: 'Rubik', sans-serif

.bg-block
  margin-top: 60px
  z-index: -1
  position: relative

  .bg-blue
    position: absolute
    background-color: #1F2951
    width: 100%
    height: 100px
    transform-origin: center
    transform: rotate(-8deg) translateX(-100px)

  .bg-grey
    top: 100px
    position: absolute
    background-color: #F2F2F2
    width: 100%
    height: 780px
    transform-origin: center
    transform: rotate(-5deg) translateY(-60px)

.pua-highlight
  background: $primary
  color: $white
  letter-spacing: 0.64px
  line-height: 25px

.header
  display: flex
  flex-direction: column
  justify-content: space-between
  margin-left: 10px

.pua-navbar
  img.logo
    height: 35px
    width: 50px
    margin-top: 30px

.pua-header
  margin-top: 100px
  width: 80%
  flex-direction: column
  z-index: 1

  @media screen and (min-width: 769px)
    width: 50%

  .logo
    margin-top: 60px

img.bubble
  position: absolute
  width: 632px
  height: 507px
  left: 35% // bottom: 0;
  top: 30%
  z-index: 0

  img
    width: 100px

.has-bg-img
  height: 640px
  background: url('/assets/header-bg.jpg') center center
  background-size: cover
  position: relative

h3.number-tag
  font-size: 45px
  color: #E4003A
  letter-spacing: 0.6px

.full-block
  font-size: 18px
  line-height: 28px
  padding: 30px 0 30px 30px

.red
  background-color: #E4003A
  color: #FFFFFF

.white
  transform: translateY(-50px)
  background-color: #FFFF

h4.section-title
  font-size: 35px
  color: #1F2951

p.quote
  font-size: 24px
  color: #1F2951
  line-height: 28px

.bloc
  padding-left: 60px
  position: relative

.association
  .white-bloc
    padding: 0 70px 27px 0
    background: white
    position: absolute

.red-block
  font-size: 27px
  letter-spacing: 0.64px
  line-height: 25px
  background-color: #E4003A
  color: white

.white-block
  background: #FFFFFF
  font-size: 20px
  color: #1F2951
  letter-spacing: 1px
  line-height: 25px
  margin-top: 10px

.blue-section
  background-color: #1F2951
  font-size: 18px
  color: #FFFFFF
  line-height: 28px
  padding: 46px

  p.light
    font-size: 13px
    color: #FFFFFF
    line-height: 23px
    margin: 30px 0

.more-info
  :before
    content: url('/assets/micro-logo.svg')
    margin-right: 10px

  margin-top: 20px
  padding-right: 20px
  background-color: #E4003A
  text-align: right
  color: #FFFF
  text-transform: uppercase

#sw
  display: flex
  justify-content: space-between
  flex-direction: column

  @media screen and (min-width: 769px)
    flex-direction: row

.blue-text
  width: 50%
  // width: 40%;
  margin-bottom: 50px

  h4
    font-size: 27px
    color: #FFFFFF
    letter-spacing: 0.64px
    line-height: 25px
    background-color: #1F2951
    margin-bottom: 15px

  p
    text-align: justify
    font-size: 13px
    color: #000000
    line-height: 20px

.sponsors
  margin-top: 50px

#footer
  margin-top: 80px

  .footer-text
    align-items: flex-end
    display: flex

  .footer-right
    justify-content: flex-end

    a
      color: white
      font-size: 2em
      text-decoration: none

      :hover
        opacity: 0.7
</style>

