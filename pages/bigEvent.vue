<template lang="pug">
  .bg 
    section.header
      .container
        .columns
          .culumn
            img(src="~assets/bigevent/logoBE.png") 
          .column.is-two-fifths
            p “Après les Startup Weekend d’Annecy, Grenoble et Chambéry,le collectif Play Up Alps rassemble l'ensemblede sa communauté à Chambéry, 
              br
              | <span class="yellow">le 23 Mai 2019, à partir de 18h</span>pour une soirée placée sous le signe de l’inspiration, de l’entreprenariat, de la réussite, et du partage.
          .culumn
        .columns
          .column
          .column.is-three-fifths
            p A travers le Big Event, Play Up Alps rassembleles petits et grands entrepreneurs de l’arc alpinainsi que les curieux de l’entreprenariat, pour se rencontrer,échanger et inspirer les réussites de demain !
          .column
      img(src="~assets/bigevent/etoileVertical.png" class="v-star is-hidden-touch") 
    section.relative
      .container-fluid
        .line
          img(src="~assets/bigevent/cisor.png" class="cisor") 
    section.speaker
      .container
        .columns
          .column.is-8.is-offset-2
            h3 PROGRAMME
            h4 Gagnants Startup Weekend
            p Que sont-ils devenus ?
            h4 Table Ronde 
              br
              | " Les étapes de l’hyper-croissance" avec :
            p Jenifer Cataldo, CEO de Vinatis   
            p Johnathan Bonzy, fondateur de Une Petite Mousse
            p Sébastien Moulis, co-fondateur de Skiply
            h4 Conférences : 
            p   "Comment passer de 0 à 1 millions en 1 an ?" par Grégoire Gambetto, co-fondateur de Germinal
            p "Et si l'humain était la clé de la croissance ?" par Stéphane Couleaud et Sophie Panot de Webmecanik
        .columns
          .column.is-8.is-offset-2.has-text-centered
              a(href="https://www.eventbrite.fr/e/billets-the-big-event-1-rendez-vous-avec-linspiration-60123075738" class="cta-speaker") Plus d’infos
                //- section 
                //-   .container 
                //-     .columns
                //-       .column.speaker-title.has-text-centered
                //-         img(src="~assets/bigevent/gregoire.png")
                //-         br
                //-         span.yellow Grégoire Gambetto
                //-         br
                //-         | Co-fondateurde Germinal
                //-       .column.speaker-title.has-text-centered
                //-         img(src="~assets/bigevent/jennifer.png")
                //-         br
                //-         span.yellow Jennifer Cataldo
                //-         br
                //-         | CEOde Vinatis
                //-       .column.speaker-title.has-text-centered
                //-         img(src="~assets/bigevent/alix.png")
                //-         br
                //-         span.yellow Alix Gauthier
                //-         br
                //-         | Co-fondateur deCopines de Voyages
                //-     .columns
                //-       .column.is-three-fifths.is-offset-one-fifth.speaker-title
                //-         span.larger et bien d’autres... 
                //-         br
                //-         |viendront partager leurs expériences entrepreneurialesautour d’une table ronde et de conférences. 
                //-         br
                //-         br
                //-         | Et parce qu’on ne change pas les bonnes habitudes… Un repas convivial autour de belles tablées vous attendpour compléter cette soirée exceptionnelle ! 
    section.insolite
          img(src="~assets/bigevent/un-lieu-insolite.png" class="title-insolite") 
          .blue-square
            .text-insolite
              h3 Play Up Alps
              h4 vous propose un événement dans un lieu inédit
                br 
                | à Chambéry pour une soirée exceptionnelle!
              h5 Et pour faire durer un peu le suspens, ce lieu insolite ne sera
                br 
                | dévoilé aux participants que quelques jours
                br
                | avant l’événement !
          a(href="https://www.eventbrite.fr/e/billets-the-big-event-1-rendez-vous-avec-linspiration-60123075738" class="cta-insolite") JE PARTICIPE
    section.reasons-section
      .container
        .columns
          .column.reasons.is-6.is-offset-3
            .yellow.big 3
            h3 bonnes raisons
              br
              | de participer
              br
              | à l’événement
        .columns
          .column.is-6.is-offset-3
            .reasons-list
              ul 
                li S'inspirer de belles 
                  br 
                  |réussites pour préparer la vôtre
                  
                li Vivre une expérience différente
                  br 
                  |et conviviale dans un lieu inédit !
                  
                li Rencontrer et échanger
                  br 
                  |avec d'autres entrepreneurs  du territoire alpin
              a(href="https://www.eventbrite.fr/e/billets-the-big-event-1-rendez-vous-avec-linspiration-60123075738" class="cta-insolite") JE PARTICIPE
      img(src="~/assets/bigevent/etoileHorizontal.png" class="reason-star is-hidden-touch")
      img(src="~/assets/bigevent/logoBE.png" class="reason-logo is-hidden-touch")
      img(src="~/assets/bigevent/logo-play-upBE.png" class="reason-logoPUA is-hidden-touch")

</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style lang="sass" scoped>
.line
  position: relative
  border-bottom: 1px #97bfe3 dashed
.cisor 
  // position: absolue
  margin-left: 70vw
  transform: translateY(65%)
.bg 
  padding-top: 60px
  width: 100vw
  height: 100%;
  background-image: linear-gradient(to right, #252c50 3%, #415b8a)
  font-family: 'Rubik', sans-serif

.v-star 
  position: absolute
  transform: translateY(-60px)
  top: 0
  right: 0

.yellow
  color: #efd938
  font-weight: bolder
.header 
  position: relative
  height: 100%
  p 
    // width: 588px;
    // height: 99px;
    font-family: Rubik;
    font-size: 23px;
    font-weight: 300;
    font-style: normal;
    font-stretch: normal;
    line-height: 1.09;
    letter-spacing: -0.5px;
    text-align: center;
    color: #ffffff;

// ----------------------------
.speaker
  padding-top: 2em
  padding-bottom: 4em
  p 
    font-family: Rubik;
    font-size: 23px;
    font-weight: 300;
    font-style: normal;
    font-stretch: normal;
    line-height: 1.15;
    letter-spacing: -0.5px;
    color: #ffffff;
    margin-left: 10px
  h4 
    font-family: Rubik;
    font-size: 25px;
    font-weight: bold;
    font-style: normal;
    font-stretch: normal;
    line-height: 1.09;
    letter-spacing: -0.5px;
    color: #ffffff;
    margin-bottom: 10px
    margin-top: 10px
    
  h3 
    font-family: Rubik;
    font-size: 37.5px;
    font-weight: bold;
    font-style: normal;
    font-stretch: normal;
    line-height: 0.96;
    letter-spacing: -0.8px;
    text-align: center;
    color: #f4e33f;
    margin-bottom: 40px
  .cta-speaker 
    font-size: 33px;
    letter-spacing: -0.7px;
    text-align: center;
    text-transform: uppercase;
    padding: 9px 19px;
    color: #252d52;
    background-image: linear-gradient(to right, #faef65, #e6c72e);

.speaker-title
  //   width: 238px;
  // height: 75px;
  // font-family: Rubik;
  font-size: 25px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.08;
  letter-spacing: -0.5px;
  text-align: center;
  color: #ffffff;
  .larger
    font-size: 37px;
    letter-spacing: -0.7px;

.cta
  font-size: 33px;
  letter-spacing: -0.7px;
  text-align: center;
  text-transform: uppercase;
  padding: 13px 23px
  color: #252d52;
  background-image: linear-gradient(to right, #faef65, #e6c72e);
  margin-bottom: 2em

.insolite
  height: 550px
  background-image: url('~assets/bigevent/insoliteBGoverlay.jpg')
  background-size: cover
  background-position: center
  padding-top: 50px
  display: flex
  flex-direction: column
  justify-content: center
  align-items: center

.blue-square
  height: 270px
  position relative
  width: 60%
  box-shadow: -2.1px -2.1px 0 0 #ffffff;
  background-image: linear-gradient(to right, #5980b1 1%, #aed5f3)
  transform: translateY(-52px) rotate(-8.5deg)
  z-index: 0
  text-align: center;
  color: #ffffff;
  .text-insolite
    margin-top: 30px
    transform: rotate(8.5deg)
    h3 
      font-size: 32px;
      font-weight: bold;
      line-height: 0.97;
      letter-spacing: -0.6px;
    h4 
      font-size: 30px;
      line-height: 1.03;
      letter-spacing: -1.2px;
      margin-bottom: 20px
    h5 
      font-size: 24px;
      line-height: 1.1;
      letter-spacing: -0.6px;

.title-insolite
  z-index: 1
.cta-insolite
  font-size: 33px;
  letter-spacing: -0.7px;
  text-align: center;
  text-transform: uppercase;
  padding: 9px 19px
  color: #252d52;
  background-image: linear-gradient(to right, #faef65, #e6c72e);
  transform: translateY(-70px)
.reasons-section
  position: relative
  padding: 50px 0
.reason-star
  position: absolute
  bottom: 0
.reason-logo
  position: absolute
  top: 20px
  right: 50px
  height: 200px
.reason-logoPUA
  position: absolute
  bottom: 50px
  right: 250px
  height: 100px
.reasons
  display: flex
  justify-content: center
  .big 
    width: 95px;
    height: 111px;
    font-family: Rubik;
    font-size: 156.5px;
    font-weight: bold;
    font-style: normal;
    font-stretch: normal;
    line-height: 0.6;
    letter-spacing: -3.1px;
    text-align: center;
    margin: 12px 20px 0 0

  h3
    font-family: Rubik;
    font-size: 42px;
    font-weight: bold;
    font-style: normal;
    font-stretch: normal;
    line-height: 0.88;
    letter-spacing: -0.8px;
    text-align: left;
    color: #ffffff;
.reasons-list
  padding-left: 250px
  li
    font-family: Rubik;
    font-size: 22.5px;
    font-weight: normal;
    font-style: normal;
    font-stretch: normal;
    line-height: 1;
    letter-spacing: -0.5px;
    text-align: left;
    color: #ffffff;
    margin-bottom: 20px
    &:before
      content: "-"
      height: 10px
      padding-right: 5px

.cta-reason 
  font-size: 33px;
  letter-spacing: -0.7px;
  text-align: center;
  text-transform: uppercase;
  padding: 9px 19px
  color: #252d52;
  width: 254px;
  height: 63px;
  margin-top: 30px
  background-image: linear-gradient(to right, #faef65, #e6c72e);




</style>
