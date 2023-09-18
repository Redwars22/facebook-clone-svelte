<script>
  import InfoAreaData from './InfoAreaData.svelte'

  export let bio;
</script>

<div class="info-area-container">
  <h3>Apresentação</h3>
  <p>{bio}</p>
  <hr/>
  <div>
    <InfoAreaData icon="briefcase-fill" data="De" dataInBold="Ponta Grossa"/>
    <InfoAreaData icon="mortarboard-fill" data="De" dataInBold="Ponta Grossa"/>
    <InfoAreaData icon="house-door-fill" data="De" dataInBold="Ponta Grossa"/>
    <InfoAreaData icon="geo-alt-fill" data="De" dataInBold="Ponta Grossa"/>
    <InfoAreaData icon="heart-fill" data="De" dataInBold="Ponta Grossa"/>
    <InfoAreaData icon="clock-fill" data="De" dataInBold="Ponta Grossa"/>
  </div>
</div>

<style>
  .info-area-container {
    color: #cac6cb;
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    background-color: #242526;
    padding: 5px 10px 5px 10px;
    border-radius: 15px;
    margin: 15px;
  }

  p {
    color: #cac6cb;
  }

  hr {
    border-color: #3a3b3c;
    color: #3a3b3c;
  }
</style>