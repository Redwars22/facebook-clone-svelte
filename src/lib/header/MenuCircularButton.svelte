<script>
  export let icon;
</script>

<a href="">
  <i class="bi bi-{icon} icon"></i>
</a>

<style>
  a {
    background-color: #333434;
    border-radius: 50%;
    color: #3a3b3c;
    display: flex;
    width: 43px;
    justify-content: center;
    align-items: center;
  }

  a:hover {
    background-color:  #3a3b3c;
  }

  .icon {
    font-size: 1.25rem;
    color: #e4e6eb;
    padding: 5px;
  }
</style>