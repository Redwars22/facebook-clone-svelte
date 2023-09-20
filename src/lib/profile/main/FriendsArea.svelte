<script>
  export let friends = [];
</script>

<div class="friends-area-container">
  <div><h3>Amigos</h3>
  <span>Ver todos os amigos</span></div>
  <div class="friends-grid">
    {#each friends as friend}
      <span>{friend.name}</span>
    {/each}
  </div>
</div>

<style>
  .friends-area-container {
    color: #cac6cb;
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    background-color: #242526;
    padding: 5px 10px 5px 10px;
    border-radius: 10px;
    margin: 15px;
  }

  .friends-area-container > div {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }

  .friends-area-container > span {
    color: #3f84d7;
  }

  .friends-grid {
    display: grid;
    grid-template-columns: repeat(3, 33%);
  }
</style>