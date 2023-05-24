<script>
  export let text = ''

  const year = new Date().getFullYear()
</script>

<footer class="bg-dark">
  <div class="inner">
    © Copyright {year}
    {text} All rights reserved.
  </div>
</footer>

<style>
  .inner {
    padding-block: 2em;
    text-align: center;
  }
</style>
