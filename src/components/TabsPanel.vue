<template>
  <div class="animated-tabs-content">
    <b-tabs>
      <b-tab active>
        Letter Blazes Boylan Howth Head Molly Tinbad the Tailor yes I said yes I will Yes. Sandymount strand O rocks soft kidneys metempsychosis seedcake Sandycove omphalos Molly burgundy. Fortyfoot yellow Love loves to love love Poldy faintly scented urine burgundy. Song Rudy Frseeeeeeeeeeeeeeeeeeeefrong Proteus rhododendrons letter Kinch portals of discovery Poldy. La ci darem la mano song Dedalus O rocks the
      </b-tab>
      <b-tab>
        Pommy ipsum one would be honoured to know your onions bull dog pompous tallywhacker laughing gear slappers, pie-eyed treacle on the beat smeg head pulled a right corker the dog's dinner on a stag do. Ear hole macca ever so lovely what a doddle tad, twiglets knows bugger all about nowt goggledegook grub's up goggledegook, tosser absolute cotton on.
      </b-tab>
      <b-tab>
        Bacon fitness you should message me Breaking Bad. Rock climbing thinking about trying yoga Doctor Who The Daily Show joking around, honest and direct optimistic trying this for the first time my favorite word is seeing as many countries as possible. Playing my guitar introvert I value art my eyes Family Guy whiskey.
      </b-tab>
      <b-tab>
        Do you love movies as much as you love making cool websites? Then, boy – have we got the lorem ipsum for you! Our badass text generator will give you the best lines from some of the hardest Hollywood legends – we’re talking Eastwood, Caine, Carrey and Freeman – and mix them up ready to work their magic on your new website. In fact, we reckon you’ll love Picksum Ipsum so much, you might never want to replace it with real text.
      </b-tab>
    </b-tabs>
  </div>
</template>

<script>
export default {
  name: 'TabsPanel'
}
</script>

<style lang="scss">
  @import "~/_variables.scss";

  .animated-tabs-content {
    .tabs ul {
      width: 200px;
      height: 200px;
      border: none;
      background: $animatedTabsMainBg;
      left: 0;
      right: 0;
      margin: auto;
      position: relative;

      &::before {
        content: "";
        position: absolute;
        width: 150px;
        height: 150px;
        background: red;
        border-radius: 50%;
        left: 0;
        right: 0;
        top: 0;
        bottom: 0;
        margin: auto;
        background: $animatedTabsMainBg;
        z-index: 2;
      }

      li {

        &:first-child a {
          width: 100px;
          height: 100px;
          background: $animatedCircleColor;
          border-radius: 100px 0 0 0;
          top: 0;
          left: 0;

          &:hover, &.active {
            transform: translate(-8px, -7px);
          }
        }

        &:nth-child(2) a {
          width: 100px;
          height: 100px;
          background: $animatedCircleColor;
          border-radius: 0 100px 0 0;
          top: 0;
          right: 0;

          &:hover, &.active {
            transform: translate(8px, -7px);
          }
        }

        &:nth-child(3) a {
          width: 100px;
          height: 100px;
          background: $animatedCircleColor;
          border-radius: 0 0 0 100px;
          bottom: 0;
          left: 0;

          &:hover, &.active {
            transform: translate(-8px, 7px);
          }
        }

        &:nth-child(4) a {
          width: 100px;
          height: 100px;
          background: $animatedCircleColor;
          border-radius: 0 0 100px 0;
          bottom: 0;
          right: 0;

          &:hover, &.active {
            transform: translate(8px, 7px);
          }
        }

        a {
          border: none;
          position: absolute;
          transition: 100ms ease-in-out;

          &.active {
            background: $animatedCircleActive;
            box-shadow: $animatedCircleActiveShadow;
            z-index: 1;
          }
        }
      }
    }

    .tab-content {
      margin-top: 50px;
    }
  }
</style>
