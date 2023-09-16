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
  <ProfileTabButtons state="idle" title="Mais" icon="caret-down-fill"/>
</div>

<style>
  div {
    display: flex;
    border-top: 1px solid #3a3b3c;
    padding-top: 5px;
    gap: 5px;
  }
</style>