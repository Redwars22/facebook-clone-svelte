<script>
  export let icon;
  export let data;
  export let dataInBold;
</script>

<div class="container">
  <i class="bi bi-{icon}"></i>
  <div>
    <span>{data}</span>
    {#if dataInBold}<strong>{dataInBold}</strong>{/if}
  </div>
</div>

<style>
  i {
    color: #8c939d;
    font-size: 1.5rem;
  }

  .container {
    color: #cac6cb;
    margin-top: 10px;
    margin-bottom: 10px;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  span, strong {
    font-size: 1rem;
  }
</style>