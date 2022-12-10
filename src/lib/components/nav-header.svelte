<script lang="ts">
  export let targets: { label: string; id: string }[];
</script>

<header>
  <img class="logo" src="ssm-logo-landscape.svg" alt="" />
  <button>
    メニュー
    <div class="arrow">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
        <path d="M12 2 4.5 20.29l.71.71L12 18l6.79 3 .71-.71z" />
      </svg>
    </div>
  </button>
</header>

<style lang="stylus">
  header
    box-sizing border-box
    display flex
    align-items center
    justify-content space-between
    width 100%
    height 4rem
    padding 0 (@height / 2)
    background-color #fff
  .logo
    height 60%
  button
    display flex
    align-items center
    height 100%
    padding 0
    margin 0
    font-size 1.2em
    background-color #fff0
    border none
    color #333
  .arrow
    box-sizing border-box
    display grid
    place-items center
    height 55%
    aspect-ratio 1
    margin-left 1ch
    background-color #f7931e
    border-radius 40%
    svg
      height 50%
      fill #fff
      rotate 45deg
</style>
