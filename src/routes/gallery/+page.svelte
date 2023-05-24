<script>
  import Card from "$lib/Card.svelte";
  import PageTitle from "$lib/PageTitle.svelte";

  export let data

  console.log(data)
</script>

<PageTitle title="Gallery" />

<ul class="auto-grid">
	{#each data.posts.posts as post}
		<Card {post} buttonText="Read More" />
	{/each}
</ul>
