<template lang="pug">
div
  section.has-bg-img
    .container
      .header
        .pua-navbar
          a(href="/")
            img.logo(src="~assets/logo.png")
        .pua-header
          .blue-block 
            .event-title Startup Weekend Grenoble #9
          .dates 29/11 - 01/12 2019 
          .location Grenoble École de Management
          .more-info.big
            a(href="https://www.eventbrite.com/e/startup-weekend-grenoble-9-tickets-76968598149")
              |Je participe
          #eventbrite-widget-container-76968598149.eventbrite
    .columns
      .column 
      .column
        .full-block.fixed
          ul
            li
              a(href="#section-what")
                |C'est quoi ?
            li
              a(href="#section-who")
                |C'est pour qui
  section#section-what
    .container
      h3.number-tag #  C'EST QUOI ?
      p.quote 1 idée pitchée en 1 minute deviendra une startup 54h plus tard...
      p En 54 heures, vous allez expérimenter les hauts, les bas, les moments d'euphories et de doutes qui jalonnent la création et la vie d'une startup.
      p En participant au Startup Weekend, vous allez vivre une expérience unique sur la création d'une startup en partant parfois d'une simple idée, et accompagnés par des Coachs expérimentés qui seront là pour vous aider à prendre les 3bonnes décisions, pour que d'une idée puisse émerger une véritable startup !
      br
      p.quote Déroulement du week-end
      p Durant 54 heures, plus de 100 participants - étudiants, professionnels, entrepreneurs, marqueteurs, designers, développeurs, mentors et conférenciers - se réunissent pour créer des business model innovants et convaincre un jury d’experts de la viabilité de leur projet.
      br
      .columns
        .column
          p.quote Le vendredi
          p Ceux qui le souhaitent « pitchent » leur idée / projet en 60 secondes : 15 projets sont ensuite sélectionnés par les votes de tous les participants. Les porteurs de projets sélectionnés réunissent autour d’eux une équipe de 4 à 8 personnes pour développer leur idée durant tout le week-end.
        .column
          p.quote Le samedi
          p Du vendredi soir au dimanche, les participants travaillent en équipe sur la faisabilité de leur projet. Des mentors et des Coachs les accompagnent pour les guider, identifier et fiabiliser leur modèle économique, et déterminer la viabilité du projet.
        .column
          p.quote Le dimanche
          p A la fin du weekend, chaque équipe à 5 minutes pour présenter son projet devant un jury d’experts, suivi de 5 minutes de questions / réponses. Les projets les plus prometteurs sont récompensés sur la base de 3 critères : validation client, modèle économique, cohésion d’équipe et l’exécution.
          br
  section#section-who
      .container
        h3.number-tag # C'est pour qui ?
        p Événement ouvert à tous, le Startup Weekend Grenoble a pour leitmotiv la conviction que tout le monde peut créer sa startup et que l’esprit d’équipe est la clef de voûte de tous les projets.
        p Vous avez une idée ? Venez la présenter le vendredi : vous aurez alors 1 minute pour convaincre les autres participants de voter pour vous et de rejoindre votre équipe !
        p Vous n'avez pas d'idée ? Aucun soucis ! Le Startup Weekend n'est pas réservé qu'à ceux qui ont des idées : vous rejoindrez une des équipes constituées dès le vendredi soir, et apporterez votre compétence et votre motivation pour faire avancer l'idée et l'amener au stade de projet !
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

  script(src="https://www.eventbrite.com/static/widgets/eb_widgets.js")
  script.
    var exampleCallback = function() {
        console.log('Order complete!');
    };

    window.addEventListener('load', function() {
      window.EBWidgets.createWidget({
        // Required
        widgetType: 'checkout',
        eventId: '76968598149',
        iframeContainerId: 'eventbrite-widget-container-76968598149',

        // Optional
        iframeContainerHeight: 425,  // Widget height in pixels. Defaults to a minimum of 425px if not provided
        onOrderComplete: exampleCallback  // Method called when an order has successfully completed
      });
    });
</template>

<script>
export default {
  head() {
    return {
      title: "Startup Weekend Grenoble #9 · Play Up Alps"
    }
  }
}
</script>

<style lang="stylus">
body
  font-family: 'Rubik', sans-serif

ul li
  display inline

li
  padding 1rem
  font-weight bold

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
  flex-direction: column
  width 100%
  z-index: 1

  .logo
    margin-top: 60px

  .dates 
    font-size 3rem
    font-weight bold
    color white

  .location
    color white
    font-size 3rem

  .event-title
    color white
    font-weight bold
    font-size 4rem

  .eventbrite
    margin-top 30px

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
  min-height: 100vh
  background: url('/assets/header-bg.jpg') center center
  background-size: cover
  position: relative

h3.number-tag
  font-size: 45px
  color: #1078be
  letter-spacing: 0.6px
  font-weight bold
  text-transform uppercase

.full-block
  font-size: 18px
  line-height: 28px
  padding: 30px 0 30px 30px
  &.fixed
    background white
    width 100%
    position absolute
    bottom 0

.red
  background-color: #E4003A
  color: #FFFFFF

.blue
  background-color: #1078be
  color: #FFFFFF

.white
  transform: translateY(-50px)
  background-color: #FFFF

h4.section-title
  font-size: 35px
  color: #1F2951

p
  text-align justify

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


.blue-block
  font-size: 27px
  letter-spacing: 0.64px

  background-color: #1078be
  color white
  display inline-block

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
  margin-top: 20px
  padding-right: 20px
  background-color: #1078be
  text-align: right
  color: #FFFF
  text-transform: uppercase
  display inline-block

  a
    color white

  &.big
    font-size 2rem
    font-weight bold
    padding 20px

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