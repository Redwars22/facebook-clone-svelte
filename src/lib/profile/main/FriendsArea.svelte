<script>
  export let friends = [];
</script>

<div class="friends-area-container">
  <div class="header">
    <h3>Amigos</h3>
    <span>Ver todos os amigos</span>
  </div>
  <div class="friends-grid">
    {#each friends as friend}
    <div class="friend-container">
      <img src={friend.avatar} alt={friend.name}/>
      <span>{friend.name}</span>
    </div>
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

  .friend-container {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    text-align: left;
    font-size: 13px;
  }

  .friends-area-container > .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }

  .friends-area-container > div > span {
    color: #3f84d7;
    margin-top: 5px;
  }

  .friends-grid {
    display: grid;
    grid-template-columns: repeat(3, 33%);
    grid-template-rows: repeat(2, auto);
    gap: 10px;
  }

  .friend-container > img {
    border-radius: 8px;
    width: 101px;
    height: 101px;
  }
</style>