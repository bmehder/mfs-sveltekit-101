<script>
  import '$lib/app.css'
  import Header from '$lib/Header.svelte'
  import Footer from '$lib/Footer.svelte'
</script>

<div class="wrapper">
  <Header logo="MFS Art Class" />

  <main class="flow">
    <slot />
  </main>

  <Footer text="Anna Pollard." />
</div>

<style>
  .wrapper {
    min-height: 100dvh;
    display: grid;
    grid-template-rows: auto 1fr auto;
  }
  main {
    width: 100%;
    max-width: var(--max-width);
    margin-inline: auto;
    padding-block: 4rem;
    padding-inline: 2rem;
    color: var(--light);
    line-height: 1.5;
    overflow: auto; 
  }
</style>