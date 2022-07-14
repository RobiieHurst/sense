<script>
    export let title = ""
</script>

<div class="title">
    <a href="/"><img width="200px" src="/sense_logo.svg" alt="site logo"></a>
    <h1>{title}</h1>
</div>

<style>
    .title {
        display: flex;
    }
    .title img {
        display: inline-block;
    }
    .title h1 {
        margin-left: 10px;
    }
</style>