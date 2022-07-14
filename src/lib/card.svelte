<script>
    export /**
* @type {any}
*/
     let id
    export let title = "Place Holder" 
</script>

<div class="card">
    <a sveltekit:prefetch href={`/guides/${id}`}><h2>{title}</h2></a>
</div>

<style>
    .card {
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2); /* this adds the "card" effect */
        padding: 16px;
        text-align: center;
        background-color: #f1f1f1;
    }
</style>
