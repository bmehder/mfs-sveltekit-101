<script>
  export let post
  export let buttonText = 'Something'

  const { featured_image, title, excerpt, slug } = post
</script>

<li class="bg-light">
  <a href="/gallery/{slug}">
    <img class="square" src={featured_image} alt="placeholder" />
  </a>
  <div class="content">
    <a href="/gallery/{slug}">
			<h2>{@html title}</h2>
		</a>
    <p>{@html excerpt}</p>
    <a class="button" href="/gallery/{slug}">{buttonText}</a>
  </div>
</li>

<style>
  li {
    margin-inline: auto;
    list-style: none;
  }

  .content {
    display: grid;
    gap: 1.5em;
    padding: 1.5em;
  }

	.content :global(p + p) {
		margin-block-start: 1.5rem;
	}
</style>
