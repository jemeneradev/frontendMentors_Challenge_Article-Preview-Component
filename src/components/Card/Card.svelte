<script>
  import Contact from "./Contact.svelte";
  import Description from "./Description.svelte";
</script>

<style>
  .Card {
    position: relative;
    margin: 0;
    padding: 0;
    width: 327px;
    height: 512px;
    border-radius: 10px;
    /* background-color: red; */
    border-radius: 10px;

    opacity: .5;
  }

  .Card .Card__banner {
    height: 200px;
    width: 100%;
    overflow: hidden;
    border-bottom-right-radius: 0px;
    border-bottom-left-radius: 0px;
  }
  .Card .Card__banner img {
    width: 327px;
    object-position: 0px -16px;
  }
  .Card .Card__Info {
    position: relative;
    width: 100%;
    height: 313px;
  }
</style>

<article class="Card">
  <figure class="Card Card__banner">
    <img
      src="./images/drawers.jpg"
      alt="background: drawers with green background" />
    <!--  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption> -->
  </figure>
  <div class="Card Card__Info">
    <Description />
    <Contact />
  </div>
</article>
