<script lang="ts">
  import "../app.css"
  import topBgPattern from "$lib/images/bg-pattern-top.svg"
  import btmBgPattern from "$lib/images/bg-pattern-bottom.svg"
</script>

<main>
  <img class="top" src={topBgPattern} alt="bg pattern top">
  <img class="btm" src={btmBgPattern} alt="bg pattern btm">
  <slot />
</main>

<style>
  main {
    position: relative; 
    overflow: hidden;
    height: 100dvh;
    display: grid;
    place-content: center;
  }

  img {
    position: absolute;
    width: 100%;
    height: 100%;
    aspect-ratio: 1;
  }

  .top {
    top: -30%;
    left:-50%;
  }

  .btm {
    bottom:-30%;
    right:-50%;
  }

 

</style>