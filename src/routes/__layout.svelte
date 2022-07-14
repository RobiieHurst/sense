<script>
	import Title from "$lib/title.svelte";
	import "../styles/global.css";
</script>

<header>
	<nav>
		<Title />
		<div class="links">
			<a href="/">Metaverse</a>
			<a href="/">Multimedia</a>
			<a href="/">Career Enhancement</a>
			<a href="/">Tools</a>
			<a href="/about">About</a>
			<a href="/guides">Guides</a>
		</div>
	</nav>
</header>
<main>
	<div class="guides">
		<slot />
	</div>
</main>
<footer>
	<p>Copyright 2022 SENSE Education</p>
</footer>

<style>
	header {
		text-align: center;
	}
	main {
		max-width: 960px;
		margin: 20px auto;
	}
	footer {
		text-align: center;
	}
	.links {
		margin-left: auto;
	}

	.links a {
		text-decoration: none;
	}

	a:hover {
		border: 1px solid #42A5FF;
	}

	a {
		margin-left: 10px;
		padding: 8px;
		border-radius: 20px;
		border: 1px solid #FFF;
	}
	nav {
		display: flex;
		align-items: center;
		max-width: 960px;
		margin: 0 auto;
		margin-top: 20px;
		border-bottom: 2px solid grey;
	}
</style>
