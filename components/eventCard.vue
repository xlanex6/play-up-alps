<template lang="pug">
    .event-card
      .event-img
        img(:src="imgUrl")
      .event-content
        .event-city 
          h3 {{city}}
        .event-address
            h3 {{place}} 
            | {{address}}
        .event-text
            | {{text}}
        .event-date
          .day
            h3 {{date}}
          .month 
            h3 {{month}}
      a(:href="linkUrl" target="_blank").more-infos plus d'infos
  </template>


<script>
export default {
  props: {
    imgUrl: "",
    linkUrl: "",
    city: "",
    place: "",
    address: "",
    text: "",
    date: "",
    month: ""
  },
  data() {
    return {};
  }
};
</script>

<style lang="stylus" scoped>
.event-card {
  background-color: white;
  height: 210px;
  display: flex;
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

    .event-city h3 {
      background-color: #1F2951;
      line-height: 1.1;
      color: white;
      font-size: 27px;
      margin-bottom: 1em;
      width: 80%;
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
