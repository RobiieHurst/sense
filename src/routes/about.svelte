<script>
    import { scale } from 'svelte/transition';
	import { quintOut } from 'svelte/easing';
    import { draw } from 'svelte/transition';
</script>


<div transition:scale="{{duration: 500, delay: 500, opacity: 0.5, start: 0.5, easing: quintOut}}" class="about">
    <h2>About us!</h2>
    <p>ABOUT IS IS BEING COOL!</p>
    <a href="/guides">View Guides</a>
    <a href="/">Home</a>
</div>

<style>
    .about{
        text-align: center;
        display: block;
        margin: 20px auto;
    }
</style>