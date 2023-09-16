<script>
  export let profileCoverURL;
  export let name;
  export let numberOfFriends;
  export let profileURL;
  export let numberOfFollowers;
</script>

<div class="profile-container">
  <img class="profile-cover" src="{profileCoverURL}">
  <div class="profile-description">
    <img class="profile-picture" src="{profileURL}">
    <div>
      <h1>{name}</h1>
      <span>{numberOfFriends} amigos</span>
      <span>•</span>
      <span>{numberOfFollowers} seguindo</span>
    </div>
    <div>
      <button class="blue-button-stories">
        <i class="bi bi-plus"></i>
        Adicionar ao story
      </button>
      <button class="grey-button">
      <i class="bi bi-pencil"></i>
      - Editar perfil</button>
      <button class="grey-button">^</button>
    </div>
  </div>
</div>

<style>
  .profile-container {
    width: 940px;
    margin-left: auto;
    margin-right: auto;
  }

  .profile-picture {
    width: 168px;
    border-radius: 100%;
    border: 6px solid #242526;
    margin-top: -84px;
    margin-lefT: 2rem;
  }

  .profile-cover {
    width: 100%;
    height: 348px;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
  }

  .profile-description {
    width: 100%;
    display: flex;
    color: white;
  }

  button {
    height: 36px;
    font-size: 15px;
    font-weight: bold;
    color: white;
    border-radius: 5px;
    border: none;
  }

  .blue-button-stories {
    background-color: #2374e1;
  }

  .grey-button {
    background-color: #3a3b3c;
  }
</style>