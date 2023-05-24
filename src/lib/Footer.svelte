<script>
  export let text = ''

  const year = new Date().getFullYear()
</script>

<footer>
  <div class="inner">
    © Copyright {year}
    {text} All rights reserved.
  </div>
</footer>

<style>
  footer {
    background-color: #323232;
    color: white;
  }
  .inner {
    max-width: 64em;
    margin-inline: auto;
    padding-block: 2em;
    text-align: center;
  }
</style>
