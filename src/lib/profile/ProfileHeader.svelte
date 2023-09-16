<script>
  import ProfileTabNav from "./ProfileTabNav.svelte";
  
  export let profileCoverURL;
  export let name;
  export let numberOfFriends;
  export let profileURL;
  export let numberOfFollowers;
</script>

<div class="profile-container">
  <img class="profile-cover" src="{profileCoverURL}">
  <div class="profile-description">
  <div class="user-picname-container">
    <img class="profile-picture" src="{profileURL}">
    <div class="profile-info-container">
      <h1>{name}</h1>
      <div>
        <span>{numberOfFriends} amigos</span>
        <span>•</span>
        <span>{numberOfFollowers} seguindo</span>
      </div>
    </div>
    </div>
    <div class="profile-buttons-container">
      <button class="blue-button-stories">
        <i class="bi bi-plus-lg"></i>
        Adicionar ao story
      </button>
      <button class="grey-button">
        <i class="bi bi-pencil"></i>
        Editar perfil</button>
      <button class="grey-button">
        <i class="bi bi-chevron-up"></i>
      </button>
    </div>
  </div>
  <ProfileTabNav/>
</div>

<style>
  span {
    font-size: 15px;
    font-weight: bold;
    color: #acb3b8;
  }

  h1 {
    font-size: 32px;
    margin: 0;
    font-weight: bold;
    color: #e4e6eb;
  }

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
    margin-left: 2rem;
    cursor: pointer;
  }

  .profile-picture:hover {
    filter: brightness(115%);
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
    justify-content: space-between;
    align-items: flex-end;
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
  }

  .blue-button-stories {
    background-color: #2374e1;
  }

  .blue-button-stories:hover {
    background-color: #4188e8;
  }

  .grey-button {
    background-color: #3a3b3c;
  }

  .grey-button:hover {
    background-color: #4d4d4d;
  }

  .user-picname-container {
    display: flex;
  }

  .profile-buttons-container {
    margin-right: 2rem;
    height: 100px;
    display: flex;
    gap: 8px;
    align-items: center;
  }

  .profile-info-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 100px;
    align-items: flex-start;
    margin-left: 10px;
  }
</style>