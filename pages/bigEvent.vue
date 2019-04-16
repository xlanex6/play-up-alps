<template lang="pug">
  .bg 
    section.header
      .container
        .columns
          .column
            img(src="~assets/bigevent/logoBE.png") 
          .column.is-two-fifths
            p “Après les Startup Weekend d’Annecy, Grenoble et Chambéry,le collectif Play Up Alps rassemble l'ensemblede sa communauté à Chambéry, 
              br
              | <span class="yellow">le 23 Mai 2019, à partir de 18h</span>pour une soirée placée sous le signe de l’inspiration, de l’entreprenariat, de la réussite, et du partage.
          .column
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
          .column

          .column
          .column

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
  position: fixed
  top: 0
  right: 0

.yellow
  color: #efd938
  font-weight: bolder
.header 
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

</style>
