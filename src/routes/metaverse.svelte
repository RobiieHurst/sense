<script>
    import Hero from "$lib/metahero.svelte";
    import { fly } from "svelte/transition";
</script>

<Hero title="Metaverse" background_color="#fff" />

<div class="mg_outer">
    <div class="mg">
        <h1>Minecraft &amp; Google based tutoring</h1>

        <div class="row">
            <div class="column">
                <p>
                    SENSE offers a revolutionary way for learners to embrace
                    language and knowledge acquisition through a mixture of
                    gameplay and academic focused exercises.
                </p>
                <br />
                <p>
                    Through the fusion of Minecraft and Google Classroom,
                    learners are placed into a digital world that combines
                    active learning with long term knowledge retainment.
                </p>
                <br />
                <p>
                    SENSE provides effective combination of personalized online
                    tutoring through the Minecraft and Google Classroom
                    platforms to ensure that each learning experience is
                    engaging, effective and sensational.
                </p>
            </div>
            <div class="column">
                <img
                    in:fly={{ x: 200, duration: 2000 }}
                    src="/learn_with_sense_1.jpg"
                    width="400px"
                    alt="vision img"
                />
            </div>
        </div>

        <br />
    </div>
</div>

<div class="ss_outer">
    <div class="ss">
        <h1>Secure and Scholastic SENSE Server</h1>
        <div class="row">
            <div class="column">
                <img
                    in:fly={{ x: 200, duration: 2000 }}
                    src="/learn_with_sense_2.jpg"
                    width="400px"
                    alt="vision img"
                />
            </div>
            <div class="column">
                <p>
                    Students will enter a secure, private server hosted by
                    internationally renowned APEX Hosting while being monitored
                    by qualified teachers as part of safe, digital and dynamic
                    environment that ensures each student receives focused
                    teaching attention from our professional educators. The
                    servers operate on a 24-hour cycle with no downtime and
                    constant backups to ensure that all learning progress is
                    saved.
                </p>
                <br />
                <p>
                    SENSE’s server offers an endless variety of lectures, active
                    learning sessions featuring puzzles, challenges, games and
                    much more to stimulate optimal academic engagement.
                    Furthermore, unlike many conventional game-based servers,
                    SENSE provides constant moderation and supervision through
                    qualified teachers. This ensures a highly secure and content
                    appropriate server while still enabling students to enjoy
                    the endless possibilities of activities and adventures
                    available on the server.
                </p>
            </div>
            
        </div>

        <br />
    </div>
</div>

<style>
    .mg_outer {
        background-color: #fff;
    }

    .mg {
        text-align: center;
        display: block;
        margin: 50px auto;
        max-width: 1080px;
    }

    .mg p {
        text-align: left;
    }

    .mg p,
    h1 {
        color: #000;
    }

    .mg img {
        border-radius: 15%;
    }

    .ss_outer {
        background-color: #42a5ff;
    }

    .ss {
        text-align: center;
        display: block;
        margin: 50px auto;
        max-width: 1080px;
    }

    .ss p {
        text-align: left;
    }

    .ss p,
    h1 {
        color: #fff;
    }

    .ss_outer img {
        border-radius: 15%;
    }

    * {
        box-sizing: border-box;
    }

    /* Float four columns side by side */
    .column {
        float: left;
        width: 50%;
        padding: 0 50px;
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
