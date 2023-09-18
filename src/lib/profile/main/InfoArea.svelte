<script>
  import InfoAreaData from './InfoAreaData.svelte'

  export let bio;
  export let birthplace;
  export let location;
  export let fiancee;
  export let workplace;
  export let member_since;
  export let relationship_status;
</script>

<div class="info-area-container">
  <h3>Apresentação</h3>
  <p>{bio}</p>
  <div class="info-list">
    <InfoAreaData icon="briefcase-fill" data="Trabalhou na empresa" dataInBold="{workplace}"/>
    <InfoAreaData icon="mortarboard-fill" data="Frequentou" dataInBold="{workplace}"/>
    <InfoAreaData icon="house-door-fill" data="Mora em" dataInBold="{location}"/>
    <InfoAreaData icon="geo-alt-fill" data="De" dataInBold="{birthplace}"/>
    <InfoAreaData icon="heart-fill" data="{relationship_status}" dataInBold="{fiancee}"/>
    <InfoAreaData icon="clock-fill" data="Entrou em {member_since}"/>
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
    border-radius: 10px;
    margin: 15px;
  }

  .info-list {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  p {
    color: #cac6cb;
    border-bottom: 1px solid #3a3b3c;
    width: 100%;
    padding-bottom: 10px;
  }
</style>