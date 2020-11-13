<script>
  import Contact from "./Contact.svelte";
  import Description from "./Description.svelte";
</script>

<style>
  .Card {
    position: relative;
    margin: 0;
    margin-top: -9px;
    padding: 0;
    width: 327px;
    height: 500px;
    border-radius: 10px;
    /* background-color: red; */
    background-color: white;
    /* box-shadow: 0px 10px 10px grey; */
    /* opacity: .3; */
  }

  .Card__banner {
    margin: 0;
    padding: 0;
    height: 200px;
    width: 100%;
    overflow: hidden;
    /* border-bottom-right-radius: 0px;
    border-bottom-left-radius: 0px; */
    border-radius: 10px 10px 0px 0px;
  }
  .Card__banner img {
    width: 328px;
    height: 281px;
    object-position: 0px -26px;
    border-radius: 10px 10px 0px 0px;
  }
  .Card__Info {
    position: relative;
    width: 100%;
    height: 313px;
    top:0px;
  }

  @media screen and (min-width: 1440px) {
    .Card {
      display: flex;
      width: 730px;
      height: 280px;
      margin: 0;
      /* top: 139px;
      left: 331px; */
    }

    .Card__banner {
      height: 280px;
      top: 0;
      left: 0;
      width: 285px;
      border-radius: 10px 0px 0px 10px;
    }

    .Card__banner img {
      width: 348px;
      object-position: 0px 0px;
    }

    .Card__Info {
      width: 445px;
      height: 100%;
      top: 0;
      left: 0;
      flex-direction: column;
    }
  }
</style>

<article class="Card">
  <figure class="Card__banner">
    <img
      src="./images/drawers.jpg"
      alt="background: drawers with green background" />
    <!--  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption> -->
  </figure>
  <div class="Card__Info">
    <Description />
    <Contact />
  </div>
</article>
