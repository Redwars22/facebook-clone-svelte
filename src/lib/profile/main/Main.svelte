<script>
  import InfoArea from './InfoArea.svelte'

  export let profile = {
      friends: [],
      pictures: [],
      info: {
        bio: "",
        birthplace: "",
        location: "",
        fiancee: "",
        workplace: "",
        member_since: "Setembro de 2023",
        relationship_status: "Em um relacionamento aberto"
      },
      posts: []
    };
</script>

<div style="background-color: #18191a">
<div class="profile-main-page">
  <div>
    <InfoArea {...profile.info}/>
  </div>
  <div></div>
</div>
</div>

<style>
.profile-main-page {
  background-color: #18191a;
  height: 900px;
  display: grid;
  grid-template-columns: 40% 60%;
  width: 940px;
  max-width: 940px;
  margin-left: auto;
  margin-right: auto;
}
</style>