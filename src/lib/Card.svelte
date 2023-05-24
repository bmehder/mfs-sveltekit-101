<script>
  export let post
  export let buttonText = 'Something'

  const { featured_image, title, excerpt, slug } = post
</script>

<li class="bg-light">
  <a href="/gallery/{slug}">
    <img class="square" src={featured_image} alt="{title}" />
  </a>
  <div class="content flow">
    <a href="/gallery/{slug}">
			<h2>{@html title}</h2>
		</a>
    <div>{@html excerpt}</div>
    <a class="button" href="/gallery/{slug}">
      {buttonText}
    </a>
  </div>
</li>

<style>
  li {
    list-style: none;
  }
  
  .content {
    padding: var(--size);
  }

	.content :global(p + p) {
		margin-block-start: var(--size);
	}
</style>
