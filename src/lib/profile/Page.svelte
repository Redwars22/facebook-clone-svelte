<script>
  import ProfileHeader from './ProfileHeader.svelte'

  const mockData = {
    name: "Andrew Nation",
    numberOfFriends: 22,
    numberOfFollowers: 145,
    profileCoverURL: "https://ubuntucommunity.s3.dualstack.us-east-2.amazonaws.com/optimized/2X/0/0921cb27d5604b464218a64ae88a3f43c7b7371a_2_690x345.png",
    profileURL: "https://github.com/Redwars22.png"
  }
</script>

<div>
  <ProfileHeader {...mockData}/>
</div>

<style>
</style>