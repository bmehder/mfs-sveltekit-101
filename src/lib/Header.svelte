<script>
	export let logo = "Fallback"
</script>

<header>
	<div class="inner">		
		<a class="logo" href="/">{logo}</a>
		<nav>
			<ul>
				<li><a href="/">Home</a></li>
				<li><a href="/about">About</a></li>
				<li><a href="/gallery">Gallery</a></li>
				<li><a href="/contact">Contact</a></li>
			</ul>
		</nav>
	</div>
</header>

<style>
	header {
		background-color: tomato;
		color: white;
	}
	
	.inner {
		max-width: 64em;
		display: flex;
		justify-content: space-between;
		align-items: center;
		gap: 1.5em;
		margin-inline: auto;
		padding: 1.5em;
	}

	a {
		color: white;
	}
	
	.logo {
		font-size: 2rem;
		font-weight: bold;
		text-decoration: none;
	}
	
	ul {
		display: flex;
		gap: 1.5em;
		list-style: none;
	}
</style>