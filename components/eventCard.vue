
<template lang="pug">
    .event-card
      .event-img
        img(:src="dataEvent.imgUrl")
      .event-content
        .event-city {{dataEvent.city}}
        .event-address
            h3 {{dataEvent.place}} 
            | {{dataEvent.address}}
        .event-text
            | {{dataEvent.text}}
        .event-date
          .day
            h3 {{dataEvent.date}}
          .month 
            h3 {{dataEvent.month}}
      a(:href="dataEvent.linkUrl" target="_blank").more-infos plus d'infos
  </template>



<script>
export default {
  props: {
    dataEvent: {
      type: Object,
      require: true
    }
  },
  data() {
    return {};
  }
};
</script>

<style lang="stylus" scoped>
.event-card {
  font-family: 'Rubik', sans-serif;
  background-color: white;
  height: 100%;
  display: flex;
  flex-direction: column;

  @media screen and (min-width: 769px) {
    height: 210px;
    flex-direction: row;
  }

  position: relative;
  margin-bottom: 60px;

  .event-img {
    padding: 0 20px;
    margin: 0 20px;
  }

  .event-content {
    padding: 30px;
    display: flex;
    flex-direction: column;
    width: 350px;

    .event-city {
      background-color: #1F2951;
      line-height: 1.1;
      color: white;
      font-size: 27px;
      margin-bottom: 1em;
      width: 60%;
      font-weight: bold;
      letter-spacing: 1.4px;
    }

    .event-address {
      color: black;
      font-style: 21px;

      h3 {
        text-transform: uppercase;
      }
    }

    .event-date {
      position: absolute;
      top: 20px;
      right: 15px;
      text-align: right;
      height: 100%;

      .day h3 {
        color: #E4003A;
        font-family: Helvetica;
        font-size: 50px;
        margin-bottom: 0;
        line-height: 1;
      }

      .month h3 {
        font-size: 20px;
        text-transform: uppercase;
        font-weight: bold;
      }
    }
  }

  .more-infos {
    position: absolute;
    bottom: 0;
    right: 10%;
    transform: translateY(50%);
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 190px;
    height: 35px;
    color: white;
    background-color: #E4003A;
    font-size: 18px;
    line-height: 21px;
    text-transform: uppercase;
    font-weight: light;
  }
}
</style>
