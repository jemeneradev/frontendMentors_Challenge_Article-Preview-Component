<script>
  import Card from "./components/Card/Card.svelte";

  let showActive = false;
  let showDesign = true;
  let makeTransparent = true;
</script>

<style>
  .design {
    position: absolute;
    margin: 0 auto;
    margin-top: -74px;
    margin-left: -24px;
    z-index: -10;
    /*  background-color: red; */
  }
  .design img {
    margin: 0 auto;
  }
  .controls {
    position: absolute;
    bottom: 0px;
    width: 500px;
  }
  .controls ul {
    display: flex;
  }
  .controls ul li {
    list-style: none;
    display: inline;
    margin-left: 20px;
  }

  @media screen and (min-width: 1440px) {
    .design {
      margin-top: -400px;
    }
  }
</style>

{#if showDesign === true}
  <div class="design">
    {#if showActive !== true}
      <picture>
        <source
          media="(min-width:1440px)"
          srcset="./design/desktop-design.jpg" />
        <source
          media="(max-width:1439px)"
          srcset="./design/mobile-design.jpg" />
        <img src="./design/mobile-design.jpg" alt="Mobile Design" />
      </picture>
    {:else}
      <picture>
        <source
          media="(min-width:1440px)"
          srcset="./design/desktop-active-state.jpg" />
        <source
          media="(max-width:1439px)"
          srcset="./design/mobile-active-state.jpg" />
        <img src="./design/mobile-active-state.jpg" alt="Mobile Design" />
      </picture>
    {/if}
  </div>
{/if}

<main>
  <Card />
</main>

<div class="controls">
  <ul>
    <li>
      <label for="showDesign">Show Design</label>
      <input
        type="checkbox"
        id="design-show"
        bind:checked={showDesign}
        name="showDesign" />
    </li>

    <li>
      <label for="showActive">Show Active State</label>
      <input
        type="checkbox"
        id="active-show"
        bind:checked={showActive}
        name="showActive" />
    </li>
    <li>
      <label for="tranparent">Make Transparant</label>
      <input
        type="checkbox"
        id="active-show"
        bind:checked={makeTransparent}
        name="showActive" />
    </li>
  </ul>
</div>
