<script>
  import ProfilePicture from '../../../lib/header/ProfilePicture.svelte';
</script>

<div class="comment-area">
  <ProfilePicture url="https://github.com/Redwars22.png"/>
  <div class="input-and-buttons-area">
    <input type="text" placeholder="Comente...">
    <div class="buttons-area">
      <i class="bi bi-person-video3"></i>
      <i class="bi bi-emoji-smile"></i>
      <i class="bi bi-camera"></i>
      <i class="bi bi-filetype-gif"></i>
      <i class="bi bi-sticky"></i>
    </div>
  </div>
</div>

<style>
  .input-and-buttons-area {
    width: 100%;
    background-color: #3a3b3c;
    border-top-left-radius: 20px;
    border-bottom-left-radius: 20px;
    border-top-right-radius: 20px;
    border-bottom-right-radius: 20px;
    padding: 8px;
    margin: 8px 8px 8px 8px;
  }

  input {
    width: 100%;
    background-color: rgba(0, 0, 0, 0);
    border: none;
    color: #b0b3b8;
    font-size: 0.9375rem;
}

  i {
    color: #9da1a4;
    padding: 5px;
    border-radius: 100%;
    display: flex;
    align-items: center;
  }

  i:hover {
    cursor: pointer;
    background-color: #555656;
  }

  .comment-area, .input-and-buttons-area {
    display: flex;
    align-items: center;
  }

  .buttons-area {
    display: flex;
  }
</style>