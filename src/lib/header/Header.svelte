<script>
  import SearchBox from './SearchBox.svelte'
  import MenuSquareButton from './MenuSquareButton.svelte'
  import MenuCircularButton from './MenuCircularButton.svelte'
  import ProfilePicture from './ProfilePicture.svelte'
</script>

<header class="fb-header">
  <div class="fb-blue-logo">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Facebook_f_logo_%282019%29.svg/1365px-Facebook_f_logo_%282019%29.svg.png" alt="">
    </div>
  <SearchBox/>
  <div class="fb-menu-container">
    <MenuSquareButton icon="house"/>
    <MenuSquareButton icon="people"/>
    <MenuSquareButton icon="play-btn"/>
    <MenuSquareButton icon="shop"/>
    <MenuSquareButton icon="controller"/>
  </div>
  <div class="fb-right-menu-container">
    <MenuCircularButton icon="dice-4"/>
    <MenuCircularButton icon="messenger"/>
    <MenuCircularButton icon="bell"/>
    <ProfilePicture url="https://github.com/Redwars22.png"/>
  </div>
</header>

<style>
  .fb-header {
    display: flex;
    height: 56px;
    max-height: 56px;
    flex-direction: row;
    background-color: #242526;
    width: calc(100% - 25px);
    padding: 0px 15px 0px 10px;
    align-items: center;
    border-bottom: 1px solid #3a3b3c;
  }

  .fb-menu-container, .fb-right-menu-container {
    display: flex;
    justify-content: space-between;
  }

  .fb-right-menu-container {
    gap: 13px;
  }

  .fb-menu-container {
    margin-left: 30px;
    margin-right: auto;
    gap: 10px;
  }

  .fb-blue-logo > img {
    width: 40px;
    margin-right: 10px;
  }
</style>