<script>
  import ProfileTabButtons from "./ProfileTabButtons.svelte";
</script>

<div>
  <ProfileTabButtons state="active" title="Publicações"/>
  <ProfileTabButtons state="idle" title="Sobre"/>
  <ProfileTabButtons state="idle" title="Amigos"/>
  <ProfileTabButtons state="idle" title="Fotos"/>
  <ProfileTabButtons state="idle" title="Vídeos"/>
  <ProfileTabButtons state="idle" title="Check-Ins"/>
</div>

<style>
  div {
    display: flex;
  }
</style>