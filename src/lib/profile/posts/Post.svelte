<script>
  import ProfilePicture from '../../header/ProfilePicture.svelte';

  export let useravatar;
  export let username;
  export let date;

  console.log({
    username, useravatar, date
  })
</script>

<div class="post-container">
  <div>
    <ProfilePicture url={useravatar}/>
    <span>{username}</span>
    <span>{date}</span>
  </div>
  <img/>
  <div></div>
</div>

<style>
  .post-container {
    background-color: #242526;
    border-radius: 5px;
    margin: 0px 15px 0px 15px;
    padding: 5px 10px 5px 10px;
  }
</style>