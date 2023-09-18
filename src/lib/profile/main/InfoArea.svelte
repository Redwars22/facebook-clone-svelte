<script>
  import InfoAreaData from './InfoAreaData.svelte'
</script>

<div>
  <h3>Apresentação</h3>
  <p></p>
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
  hr {
    border-color: #3a3b3c;
    color: #3a3b3c;
  }
</style>