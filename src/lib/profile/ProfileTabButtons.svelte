<script>
  export let state;
  export let title;
</script>

{#if state == "active"}
<a class="active-button">
  {title}
</a>
{/if}

{#if state == "idle"}
<a class="idle-button" href="">
  {title}
</a>
{/if}

<style>
  a {
    display: flex;
    align-items: center;
    height: 60px;
    text-decoration: none;
  }

  .idle-button {
    color: #B0B3B8;
  }

  .idle-button:hover {
    background-color: #3a3b3c;
    border-radius: 8px;
    padding: 0px 5px 0px 5px;
  }

  .active-button {
    color: #2e89ff;
    border-bottom: 3px solid #2e89ff;
  }
</style>