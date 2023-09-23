<script>
  import ProfilePicture from '../../../lib/header/ProfilePicture.svelte';
</script>

<div class="comment-area">
  <ProfilePicture url="https://github.com/Redwars22.png"/>
  <div>
    <input>
    <div>
      <i class="bi bi-person-video3"></i>
      <i class="bi bi-emoji-smile"></i>
      <i class="bi bi-camera"></i>
      <i class="bi bi-filetype-gif"></i>
      <i class="bi bi-sticky"></i>
    </div>
  </div>
</div>

<style>
  .comment-area {
    display: flex;
  }
</style>