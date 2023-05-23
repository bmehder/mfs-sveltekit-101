<script>
  import Card from "$lib/Card.svelte";
  import PageTitle from "$lib/PageTitle.svelte";

  export let data

  console.log(data)
</script>

<PageTitle title="Gallery" />

<ul>
	{#each data.posts.posts as post}
		<Card {post} buttonText="Read More" />
	{/each}
</ul>

<style>
  ul {
		max-width: 64em;
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(16em, 1fr));
		gap: 3em;
		margin-inline: auto;
		padding: 3em;
		line-height: 1.5;
	}
</style>