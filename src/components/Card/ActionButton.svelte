<script>
  export let actionHandler = () => {};
  export let active = false;
</script>

<style>
  .Card__Info__Contact__Action__Share {
    width: 32px;
    height: 32px;
   
    border-radius: 50%;
    margin: 0;
    padding: 0;
    z-index: 10;
    /* top: 8px;
    left: 26px; */
  }

  .Card__Info__Contact__Action__Share--active {
    background-color: #6d7f97;
    color: #ecf2f8;
  }

  .Card__Info__Contact__Action__Share--passive {
    background-color: #ecf2f8;
    color: #6d7f97;
  } 

  .Card__Info__Contact__Action__Share svg {
    margin: 0;
    margin-left: 9px;
    margin-top: 9px;
  }
</style>

<div class={active ? "Card__Info__Contact__Action__Share Card__Info__Contact__Action__Share--active":"Card__Info__Contact__Action__Share Card__Info__Contact__Action__Share--passive"} on:click={actionHandler}>
  <!-- <img src="./images/icon-share.svg" alt="share arrow" /> -->
  <svg xmlns="http://www.w3.org/2000/svg" width="15" height="13"><path
      style="fill:currentColor;"
      d="M15 6.495L8.766.014V3.88H7.441C3.33 3.88 0 7.039 0 10.936v2.049l.589-.612C2.59 10.294 5.422 9.11 8.39 9.11h.375v3.867L15 6.495z" /></svg>
</div>
