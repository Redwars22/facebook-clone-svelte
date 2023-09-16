<script>
  export let state;
  export let title;
  export let icon = "";
</script>

{#if state == "active"}
<a class="active-button">
  {title}
</a>
{/if}

{#if state == "idle"}
<a class="idle-button" href="">
  {title}
  {#if icon != ""}
    <i class="bi bi-{icon}"/>
  {/if}
</a>
{/if}

<style>
  a {
    display: flex;
    align-items: center;
    height: 60px;
    text-decoration: none;
    padding: 0px 10px 0px 10px;
    font-weight: bold;
  }

  .idle-button {
    color: #B0B3B8;
  }

  .idle-button:hover {
    background-color: #3a3b3c;
    border-radius: 8px;
  }

  .active-button {
    color: #2e89ff;
    border-bottom: 3px solid #2e89ff;
  }

  i {
    margin-left: 5px;
  }
</style>