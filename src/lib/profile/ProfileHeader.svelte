<script>
  export let profileCoverURL;
  export let name;
  export let numberOfFriends;
  export let numberOfFollowers;
</script>

<div>
  <img class="profile-cover" src="{profileCoverURL}">
  <div>
    <h1>{name}</h1>
    <button>+ Adicionar ao story</button>
    <button>- Editar perfil</button>
    <button>^</button>
  </div>
</div>

<style>
  .profile-cover {

  }
</style>