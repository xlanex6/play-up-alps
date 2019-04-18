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
       .is-three-fifths.is-offset-one-fifth
        h3 L’hypercroissance et l’humain:
          br 
          |vedettes de cette première édition !
      
    section 
      .container 
        .columns
          .column.speaker-title.has-text-centered
            img(src="~assets/bigevent/gregoire.png")
            br
            span.yellow Grégoire Gambetto
            br
            | Co-fondateurde Germinal
          .column.speaker-title.has-text-centered
            img(src="~assets/bigevent/jennifer.png")
            br
            span.yellow Jennifer Cataldo
            br
            | CEOde Vinatis
          .column.speaker-title.has-text-centered
            img(src="~assets/bigevent/alix.png")
            br
            span.yellow Alix Gauthier
            br
            | Co-fondateur deCopines de Voyages
        .columns
          .column.is-three-fifths.is-offset-one-fifth.speaker-title
            span.larger et bien d’autres... 
            br
            |viendront partager leurs expériences entrepreneurialesautour d’une table ronde et de conférences. 
            br
            br
            | Et parce qu’on ne change pas les bonnes habitudes… Un repas convivial autour de belles tablées vous attendpour compléter cette soirée exceptionnelle ! 
        .columns
          .column.is-three-fifths.is-offset-one-fifth.speaker-title
            .cta Plus d’infos sur le programme de la soirée
    section.insolite
      // .blue-layer

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
  height: 500px
  background-image: url('~assets/bigevent/insoliteBGoverlay.jpg')
  background-cover: cover
  background-position: center
  z-index: 0
  position: relative

.blue-layer
  height: 100%
  width: 100%
  background-image: linear-gradient(to right, #5980b1 3%, #aad1f0)
  position: absolute
  top: 0
  left: 0 
  opacity: 0.8
  z-index: 1

</style>
