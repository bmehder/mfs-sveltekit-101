<script>
  import PageTitle from '$lib/PageTitle.svelte'

  export let data
</script>

<article class="flow">
  <PageTitle title={data.post.title} />

  <img src={data.post.featured_image} alt={data.post.title} />

  <div>{@html data.post.excerpt}</div>
</article>
