<script>
  export let icon;
  export let data;
  export let dataInBold;
</script>

<div>
  <i class="bi bi-{icon}"></i>
  <span>{data}</span>
  <strong>{dataInBold}</strong>
</div>

<style>
  i {
    color: #8c939d;
    font-size: 1.5rem;
  }

  div {
    color: #cac6cb;
  }

  span, strong {
    font-size: 1rem;
  }
</style>