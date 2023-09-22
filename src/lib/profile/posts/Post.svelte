<script>
  import ProfilePicture from '../../header/ProfilePicture.svelte';

  export let useravatar;
  export let username;
  export let date;
  export let picture;
  export let legend;

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
  </div>
  <div class="picture-and-legend">
    <p>{legend}</p>
    <img src={picture}/>
  </div>
  <div></div>
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
</style>