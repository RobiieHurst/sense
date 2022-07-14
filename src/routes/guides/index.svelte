<script context="module">
	// @ts-ignore
	export async function load({ fetch }) {
		const res = await fetch("https://jsonplaceholder.typicode.com/posts");
		const guides = await res.json();

		if (res.ok) {
			return {
				props: {
					guides,
				},
			};
		}

		return {
			status: res.status,
			error: new Error("Could not fectch the guides"),
		};
	}
</script>

<script>
	import Card from "$lib/card.svelte";

	export /**
	 * @type {any}
	 */
	let guides;
</script>

<div class="guides">
	<ul>
		{#each guides as guide}
			<li>
				<Card id={guide.id} title={guide.title} />
			</li>
		{/each}
	</ul>
</div>

<style>
	.guides {
		margin-top: 20px;
	}

	ul {
		list-style-type: none;
		padding: 0;
	}

	a {
		display: inline-block;
		margin-top: 10px;
		padding: 10px;
		border: 1px dotted rgba(255, 255, 255, 0.2);
	}
</style>
