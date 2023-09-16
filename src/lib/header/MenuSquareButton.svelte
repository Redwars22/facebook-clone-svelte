<script>
  export let icon;
</script>

<a href="" alt="AAAA">
  <i class="bi bi-{icon} icon"></i>
</a>

<style>
  .icon {
    color: #B0B3B8;
    font-size: 1.5rem;
  }

  a {
    display: flex;
    min-width: 107px;
    width: 107px;
    height: 48px;
    max-width: 107px;
    border-radius: 8px;
    justify-content: center;
    align-items: center;
  }

  a:hover {
    background-color:  #3a3b3c;
  }
</style>