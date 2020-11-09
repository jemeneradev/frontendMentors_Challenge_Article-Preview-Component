<script>
  export let actionHandler = () => {};
</script>

<style>

  .Card__Info__Contact__Action__Share {
    width: 32px;
    height: 32px;
    background-color: #ECF2F8;
    border-radius: 50%;
    margin: 0;
    padding: 0;
    /* top: 8px;
    left: 26px; */
  }

  .Card__Info__Contact__Action .Card__Info__Contact__Action__Share img {
    margin: 0;
    margin-left: 9px;
    margin-top: 9px;
  }
</style>

<div
  class="Card__Info__Contact__Action__Share"
  on:click={actionHandler}>
  <img src="./images/icon-share.svg" alt="share arrow" />
</div>
