<script context="module">
	// @ts-ignore
	export function load({ error }) {
		return {
			props: { message: error.message }
		};
	}
</script>
    
<script>
    export /**
* @type {any}
*/
     let message
</script>

<div class="error">
    <h2>Ooops</h2>
    <p>{message}</p>
    <a href="/guides">View all guides...</a>
</div>

<style>
    .error {
        text-align: center;
        margin-bottom: 60px;
    }
</style>