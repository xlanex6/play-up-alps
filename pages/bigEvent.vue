<template lang="pug">
  .bg 
    section.header
      .container
        .columns
          .column
            img(src="~assets/bigevent/logoBE.png") 
          .column
            p.para-top “Après les Startup Weekend d’Annecy, Grenoble et Chambéry,le collectif Play Up Alps rassemble l'ensemblede sa communauté à Chambéry,le 23 Mai 2019, à partir de 18hpour une soirée placée sous le signe de l’inspiration, de l’entreprenariat, de la réussite, et du partage.
        .columns
          .column
          .column.is-three-fifths
            p A travers le Big Event, Play Up Alps rassembleles petits et grands entrepreneurs de l’arc alpinainsi que les curieux de l’entreprenariat, pour se rencontrer,échanger et inspirer les réussites de demain !
          .column
      img(src="~assets/bigevent/etoileVertical.png" class="v-star widescreen") 
    img(src="~assets/bigevent/cisor.png" class="cisor") 
    

</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style lang="sass" scoped>
.para-top 
  width: 363px;
  height: 237px;
.cisor 
  margin-left: 70vw
  transform: translateY(-50%)
.bg 
  padding-top: 60px
  width: 100vw
  height: 100vh;
  background-image: linear-gradient(to right, #252c50 3%, #415b8a)

.v-star 
  position: fixed
  top: 0
  right: 0
.header 
  position: relative
  height: 488px
  border-bottom: 1px #97bfe3 dashed
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
</style>
