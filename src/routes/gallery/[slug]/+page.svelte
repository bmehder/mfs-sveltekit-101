<script>
  import PageTitle from '$lib/PageTitle.svelte'

  export let data
</script>

<div class="post">
  <PageTitle title={data.post.title} />

  <img src={data.post.featured_image} alt={data.post.title} />

  <div class="content">
    {@html data.post.excerpt}
  </div>
</div>