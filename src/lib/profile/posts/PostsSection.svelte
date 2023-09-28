<script>
  import Post from './Post.svelte';

  export let posts = [
        {
          useravatar: "https://github.com/Redwars22.png",
          username: "Andrew Nation",
          date: "24 de Setembro às 22:43",
          legend: "Andrew TC 2023 Keynote è statu n sucessu assolutu!!!",
          picture: "https://th.bing.com/th/id/R.dddc885929b5b0a7b0f362379a11295c?rik=pfLvvpt01bIANw&pid=ImgRaw&r=0g",
          likes: 8881,
          shares: 98765
        },
        {
          useravatar: "https://github.com/Redwars22.png",
          username: "Andrew Nation",
          date: "24 de Setembro às 12:16",
          legend: "Aju ad ammettere ca C# ha ribbentatu una re lenguage e prugrammazione faurite a mmi.",
          picture: "https://th.bing.com/th/id/OIP.fO-DvZrWlhbRfVMCwH7iYQHaE8?pid=ImgDet&rs=1",
          likes: 4443,
          shares: 9871
        },
        {
          useravatar: "https://github.com/Redwars22.png",
          username: "Andrew Nation",
          date: "23 de Setembro às 11:10",
          legend: "Windows 12 sarrà veramente meju ca Windows 10? Windows 11 un è statu n sistiema operatiù fallitu, ma aju sentitu ca l'è un po chiù pesante ca Windows 10, speciarmente n PC ca possieronu na mpustazione un assé forte.",
          picture: "https://th.bing.com/th/id/OIP._70F4TLXGHSx6I8MBcr8MgHaEf?pid=ImgDet&rs=1",
          likes: 9875,
          shares: 1123
        },
        {
          useravatar: "https://github.com/Redwars22.png",
          username: "Andrew Nation",
          date: "22 de Setembro às 19:04",
          legend: "A ferramienta chiù mpurtante e usata n Windows sarrà morta da Microsoft brevemente! 🥹",
          picture: "https://th.bing.com/th/id/R.080c1599c40d1832bb1a77b8c579fa95?rik=z8yrN4Pk2DmTtw&pid=ImgRaw&r=0",
          likes: 415,
          shares: 77
        },
        {
          useravatar: "https://github.com/Redwars22.png",
          username: "Andrew Nation",
          date: "22 de Setembro às 11:04",
          legend: "Ammulannu coe miliore amice nto parcu e l'ammusamientu 🎡🥳🎉🪅😃 Aju bisognu e ammittere c'aju paore, assé paore, ma accussì me ce vadu.",
          picture: "https://funspotamericaatlanta.com/wp-content/uploads/2018/06/Ferris-Wheel-5.jpg",
          likes: 125,
          shares: 12
        }
      ];
</script>

<div>
  <div class="header">
    <div>
      <h3>Publicações</h3>
      <button>
        <i class="bi bi-sliders"></i>
        Filtros
      </button>
    </div>
  </div>
  <div>
    {#each posts as post}
      <Post {...post}/>
    {/each}
  </div>
</div>

<style>
  .header {
    color: #cac6cb;
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    background-color: #242526;
    padding: 5px 10px 5px 10px;
    border-radius: 10px;
    margin: 15px;
  }

  button {
    height: 36px;
    font-size: 15px;
    font-weight: bold;
    color: white;
    border-radius: 5px;
    border: none;
    padding: 5px 15px 5px 15px;
    cursor: pointer;
    background-color: #3a3b3c;
  }

  .header > div {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }
</style>