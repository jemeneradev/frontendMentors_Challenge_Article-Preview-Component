<script>
  import Card from "./components/Card/Card.svelte";
</script>

<style>
  .design {
    position: absolute;
    margin: 0 auto;
    margin-top: -586px;
    margin-left: -24px;
    z-index: -10;
    /*  background-color: red; */
  }
  .design img {
    margin: 0 auto;
  }

  @media screen and (min-width: 1440px) {
    .design {
      margin-top: -400px;
    }
  }
</style>

<main>
  <Card />
  <div class="design">
 <!--    <picture>
      <source media="(min-width:1440px)" srcset="./design/desktop-design.jpg" />
      <source media="(max-width:1439px)" srcset="./design/mobile-design.jpg" />
      <img src="./design/mobile-design.jpg" alt="Mobile Design" />
	</picture> -->
	<!-- <picture>
		<source media="(min-width:1440px)" srcset="./design/desktop-active-state.jpg" />
		<source media="(max-width:1439px)" srcset="./design/mobile-active-state.jpg" />
		<img src="./design/mobile-active-state.jpg" alt="Mobile Design" />
	  </picture> -->
  </div>
</main>
