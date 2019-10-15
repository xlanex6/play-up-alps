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
        iframeContainerHeight: 550,  // Widget height in pixels. Defaults to a minimum of 425px if not provided
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
    margin-top 50px

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