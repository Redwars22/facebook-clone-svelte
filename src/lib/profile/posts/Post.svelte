<script>
  import ProfilePicture from '../../header/ProfilePicture.svelte';
  import Comment from '../main/Comment.svelte';

  export let useravatar;
  export let username;
  export let date;
  export let picture;
  export let legend;
  export let likes;
  export let shares;

  console.log({
    username, useravatar, date
  })
</script>

<div class="post-container">
  <div class="horizontal-flex">
    <ProfilePicture url={useravatar}/>
    <div class="vertical-flex">
      <span class="username">{username}</span>
      <span class="date">{date} · <i class="bi bi-globe-americas"></i></span>
    </div>
    <button class="more">
      <i class="bi bi-three-dots"></i>
    </button>
  </div>
  <div class="picture-and-legend">
    <p>{legend}</p>
    <img src={picture}/>
  </div>
  <div class="space-between">
    <div>
      <i class="bi bi-hand-thumbs-up-fill blue-icon"></i>
      <i class="bi bi-heart-fill red-icon"></i>
      <span>{likes}</span>
    </div>
    <div>
      <span>{shares}</span>
      <i class="bi bi-send-arrow-up-fill"></i>
    </div>
  </div>
  <div class="action-buttons">
    <button class="post-action-buttons">
    <i class="bi bi-hand-thumbs-up"></i>
      <span>Curtir</span>
    </button>
    <button class="post-action-buttons">
      <i class="bi bi-chat"></i>
      <span>Comentar</span>
    </button>
    <button class="post-action-buttons">
      <i class="bi bi-send-arrow-up"></i>
      <span>Compartilhar</span>
    </button>
  </div>
  <div>
    <Comment/>
  </div>
</div>

<style>
  .post-container {
    background-color: #242526;
    border-radius: 10px;
    margin: 10px 15px 10px 15px;
    padding: 5px 10px 5px 10px;
    color: #e4e6eb;
  }

  .username {
    font-weight: 700;
    font-size: 15px;
  }

  .space-between, .action-buttons {
    border-bottom: 1px solid #3a3b3c;
  }

  .action-buttons {
    margin-top: 8px;
    padding-bottom: 8px;
  }

  .space-between {
    display: flex;
    justify-content: space-between;
    margin: 5px 15px 5px 15px;
    padding-bottom: 10px;
  }

  .more {
    border-radius: 100%;
    padding: 8px;
    font-size: 20px;
    color: white;
    background-color: #242526;
    margin-left: auto;
    border: none;
  }

  .more:hover {
    background-color: #3a3b3c;
    cursor: pointer;
  }

  .date {
    font-size: 13px;
    color: #a1a3a8;
  }

  .vertical-flex {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin-left: 10px;
    gap: 5px;
  }

  .horizontal-flex {
    display: flex;
    align-items: center;
  }

  img {
    width: calc(100% + 20px);
    margin-left: -10px;
  }

  .picture-and-legend {
    margin-top: 10px;
    margin-bottom: 10px;
  }

  .picture-and-legend > p {
    text-align: left;
  }

  .post-action-buttons {
    background-color: rgba(0, 0, 0, 0);
    font-size: 1rem;
    color: #b0b3b8;
    font-weight: bold;
    padding-top: 5px;
    padding-bottom: 5px;
    width: 161px;
    height: 44px;
    cursor: pointer;
    border: none;
    border-radius: 5px;
  }

  .post-action-buttons:hover {
    background-color: #3a3b3c;
  }

  .blue-icon, .red-icon {
    border-radius: 100%;
    padding: 3px;
    font-size: 12px;
  }

  .blue-icon {
    background-color: #14a4fa;
    z-index: 999999;
  }

  .red-icon {
    background-color: #ef3856;
    margin-left: -8px;
  }
</style>