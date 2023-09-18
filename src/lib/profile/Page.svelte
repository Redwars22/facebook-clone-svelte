<script>
  import ProfileHeader from './ProfileHeader.svelte'
  import Main from './main/Main.svelte'

  const mockData = {
    name: "Andrew Nation",
    numberOfFriends: 22,
    numberOfFollowers: 145,
    profileCoverURL: "https://ubuntucommunity.s3.dualstack.us-east-2.amazonaws.com/optimized/2X/0/0921cb27d5604b464218a64ae88a3f43c7b7371a_2_690x345.png",
    profileURL: "https://github.com/Redwars22.png",
    profile: {
      friends: [],
      pictures: [],
      info: {
        bio: "Busque a sua felicidade hoje, amanha e sempre!"
      },
      posts: []
    }
  }
</script>

<div>
  <ProfileHeader {...mockData}/>
  <Main {...mockData.profile}/>
  <a class="send-message-button" href="/">
    <i class="bi bi-pencil-square"/>
  </a>
</div>

<style>
  .send-message-button {
    width: 48px;
    height: 48px;
    background-color: #3a3b3c;
    display: flex;
    border-radius: 100%;
    align-items: center;
    justify-content: center;
    position: fixed;
    bottom: 15px;
    right: 15px;
  }

  .send-message-button > i {
    font-size: 1.5rem;
    color: #B0B3B8;
  }
</style>