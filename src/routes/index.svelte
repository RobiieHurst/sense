<script>
    import Card from "$lib/card.svelte";
</script>

<div class="index">
    <!-- <p>
        stuff
    </p> -->

    <div class="row">
        <div class="column">
            <Card id=1 title="Test"/>
        </div>
        <div class="column">
            <Card id=1 title="Test"/>
        </div>
        <div class="column">
            <Card id=1 title="Test"/>
        </div>
        <div class="column">
            <Card id=1 title="Test"/>
        </div>
    </div>

    <!-- <a href="/guides">View Guides</a>
    <a href="/about">About</a> -->
</div>

<style>
    .index {
        text-align: center;
        display: block;
        margin: 20px auto;
    }

    * {
        box-sizing: border-box;
    }

    /* Float four columns side by side */
    .column {
        float: left;
        width: 25%;
        padding: 0 10px;
    }

    /* Remove extra left and right margins, due to padding in columns */
    .row {
        margin: 0 -5px;
    }

    /* Clear floats after the columns */
    .row:after {
        content: "";
        display: table;
        clear: both;
    }

    /* Responsive columns - one column layout (vertical) on small screens */
    @media screen and (max-width: 600px) {
        .column {
            width: 100%;
            display: block;
            margin-bottom: 20px;
        }
    }
</style>
