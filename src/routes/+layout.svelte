<script>
  import '$lib/app.css'
  import Footer from '$lib/Footer.svelte'
  import Header from '$lib/Header.svelte'
</script>

<div class="wrapper">
  <Header logo="Art Class Gallery" />

  <main>
    <slot />
  </main>

  <Footer text="Anna Pollard" />
</div>

<style>
  .wrapper {
    min-height: 100dvh;
    display: grid;
    grid-template-rows: auto 1fr auto;
  }
  main {
    width: 100%;
    max-width: 64em;
    margin-inline: auto;
    padding: 2rem;
    line-height: 1.5;
    overflow: auto; 
    color: white;
  }
</style>