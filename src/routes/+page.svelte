<script lang="ts">
  import banner from "$lib/images/bg-pattern-card.svg"
  import avatar from "$lib/images/image-victor.jpg"
</script>


<article>
  <header>
    <img class="banner" src={banner} alt="buble pattern">
    <img class="avatar" src={avatar} alt="victor">
  </header>
  <section>
    <span class="bold">Victor Cress <span class="light">26</span></span>
    <p class="light">London</p>
  </section>
  <footer>
    <p class="bold">80K</p>
    <p class="bold">803K</p>
    <p class="bold">1.4K</p>
    <p class="light">Followers</p>
    <p class="light">Likes</p>
    <p class="light">Photos</p>
  </footer>
</article>


<style>
  article {
    background-color: whitesmoke;
    border-radius: 1rem;
    overflow: hidden;
    z-index: 5;
    max-width: 25rem;
    margin-inline: 2rem;
    min-height: 28rem;
    display: grid;
    justify-items: center;
    grid-template-rows: 2fr 2fr 1fr;
  }

  header {
    position: relative;
    /* border: 1px solid red; */
  }

  .banner {
    min-height: 4rem;
    height: 100%;
  }

  .avatar {
    border-radius: 50%;
    border: 6px solid whitesmoke;
    position: absolute;
    bottom: 0;
    left: 50%;
    translate: -50% 50%;
  }

  section {
    margin-top: 2rem;
    /* border: 1px solid red; */
    align-self: center;
  }

  footer {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    place-content: center;
    gap:1rem;
    /* border: 1px solid red; */
    border-top: 1px solid gainsboro;
    padding-inline: 2rem;
    width: 100%;
    
    
  }

  .bold {
    font-weight: var(--fw-bold);
  }

  .light {
    font-weight: var(--fw-light);
    color: var(--clr-primary-3)
  }

  p {
    text-align: center;
  }

</style>