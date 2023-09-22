<script>
  import Post from './Post.svelte';

  export let posts = [];
</script>

<div>
  <div class="header">
    <div>
      <h3>Publicações</h3>
      <button>
        <i class="bi bi-sliders"></i>
        Filtros
      </button>
    </div>
  </div>
  <div>
    {#each posts as post}
      <Post {...post}/>
    {/each}
  </div>
</div>

<style>
  .header {
    color: #cac6cb;
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    background-color: #242526;
    padding: 5px 10px 5px 10px;
    border-radius: 10px;
    margin: 15px;
  }

  button {
    height: 36px;
    font-size: 15px;
    font-weight: bold;
    color: white;
    border-radius: 5px;
    border: none;
    padding: 5px 15px 5px 15px;
    cursor: pointer;
    background-color: #3a3b3c;
  }

  .header > div {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }
</style>