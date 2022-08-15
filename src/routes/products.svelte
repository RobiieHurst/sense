<script>
    import Hero from "$lib/productshero.svelte";
    import Products from "../lib/products.svelte";
</script>

<svelte:head>
    <script src="https://code.jquery.com/jquery-2.1.0.js"></script>
    <script
        src="https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"></script>
</svelte:head>

<Hero />

<div class="prod">
    <input id="prod-a" type="checkbox" checked="true" />
    <label for="prod-a">
        <p class="prod-heading">Service Requirements</p>
        <div class="prod-arrow" />
        <p class="prod-text">
            SENSE can only offer its M&amp;G tutoring service to students that
            can meet the following technological specifications:
        </p>
        <ul>
            <li>
                <p class="prod-text">
                    A Windows 10 enabled desktop/laptop with a minimum of a 3.5
                    GHz processor, 12GB of RAM (8GB of RAM is acceptable but may
                    lead to slight lag or delays when switching between
                    Minecraft and Google Services during lessons) and a 2GB
                    graphics card (integrated graphics cards are acceptable but
                    dedicated ones will ensure more stable performance).
                </p>
            </li>
            <li>
                <p class="prod-text">
                    A stable internet connection with at least 10Mbps download
                    and upload speeds.
                </p>
            </li>
            <li>
                <p class="prod-text">
                    A pre-purchased Minecraft account with Minecraft Java
                    Edition.
                </p>
            </li>
            <li><p class="prod-text">A registered Google account</p></li>
        </ul>
    </label>
</div>

<div class="section">
    <h1>Pricing</h1>
    <Products class="prod-tiles" />
    <div class="prod">
        <input id="prod-b" type="checkbox" />
        <label for="prod-b">
            <p class="prod-heading">SENSE M&amp;G Active Tutoring Prices</p>
            <div class="prod-arrow" />
            <p class="prod-text">
                SENSE’s M&amp;G Active Tutoring lessons are priced at $39 per
                lesson no matter what subject, grade or curriculum. Lessons last
                for a 45-minute timespan with 40 minutes of direct teaching time
                and active learning. Students will be provided with materials to
                revise &amp; prepare before the lesson starts and the entirety
                of the lesson is conducted using SENSE’s unique M&amp;G active
                learning tools.
            </p>
            <p class="prod-text">
                During the lesson, students will receive access to the SENSE
                server for any activities and teaching that will take place.
            </p>
        </label>
        <input id="prod-c" type="checkbox" />
        <label for="prod-c">
            <p class="prod-heading">SENSE M&amp;G Complete Tutorings</p>
            <div class="prod-arrow" />
            <p class="prod-text">
                SENSE’s M&amp;G Complete Tutoring lessons are priced at $49 per
                lesson no matter what subject, grade or curriculum.
            </p>
            <p class="prod-text">
                Students are provided with a lesson plan detailing the outline
                and objectives of the lesson. Lessons last for a 75-minute
                timespan with a minimum of 60 minutes direct teaching time and
                active learning. Students are provided with materials before and
                after the lesson for either personal revision or as homework for
                future lessons.
            </p>
            <p class="prod-text">
                Parents are provided with an after-lesson report for each and
                every lesson.
            </p>
            <p class="prod-text">
                During the lessons, students will receive access to the SENSE
                server for any activities and teaching that will take place.
            </p>
        </label>
        <input id="prod-d" type="checkbox" />
        <label for="prod-d">
            <p class="prod-heading">SENSE Secure Teacher Moderated Server</p>
            <div class="prod-arrow" />
            <p class="prod-text">
                Students are required to have at least one lesson per month (30
                day period) with SENSE in order to qualify for the subscription
                to the SENSE server. Access to the SENSE server includes the
                Student Centre and Survival Zone along with constant moderation
                by qualified teachers to enforce a fair and safe digital
                environment.
            </p>
            <p class="prod-text">
                Students and parents wishing to having access to the server
                after the lesson may choose one of the following subscription
                models.*
            </p>
            <p class="prod-text">
                <strong>
                    Core access - $9 per month for access to the SENSE server
                    for students to build their own projects or collaborate with
                    other students. At this tier, teachers monitor the server
                    and immediately take disciplinary action against any
                    bullying, harassment or griefing.*
                </strong>
            </p>
            <p class="prod-text">
                (*Griefing refers to the intentional destruction or vandalizing
                of another player’s digital property or creation.)
            </p>
            <p class="prod-text">
                <strong>
                    Premium access - $19 per month with all the benefits of Core
                    Access. Students on Core access plus can also submit project
                    resource requests to the teacher for any collaborative
                    projects they are wanting to start. Teachers are allowed to
                    assign a certain amount of resources depending on the
                    students’ projects &amp; their intended purpose. Students on
                    premium access can request daily consultations (10-15 minute
                    meetings with up to 5 consultations per month) with teachers
                    for any projects or academic queries relating to either
                    previous or upcoming SENSE lessons.
                </strong>
            </p>
            <p class="prod-text">
                *SENSE believes in maintaining a healthy balance between digital
                and physical reality. Access to the SENSE server for every
                student is limited to 180 minutes on the server each day (lesson
                time not counting). After the 180 minutes, student progress will
                be saved and students will be ejected from the server until the
                next day. Parents can request additional or lower server access
                time based on their preferences.
            </p>
        </label>
    </div>
</div>

<div class="section">
    <h1>Additionals</h1>
    <div class="prod">
        <input id="prod-e" type="checkbox" />
        <label for="prod-e">
            <p class="prod-heading">Sign-up Special (One plus One)</p>
            <div class="prod-arrow" />
            <p class="prod-text">
                For our first-time customers, purchase your very first SENSE
                M&amp;G Complete Tutoring lesson and the second one is
                completely free. We believe in the quality and potential of our
                learning model so if th
            </p>
        </label>
        <input id="prod-f" type="checkbox" />
        <label for="prod-f">
            <p class="prod-heading">Monthly Specials</p>
            <div class="prod-arrow" />
            <p class="prod-text">
                SENSE offers monthly packages for the Complete Tutoring
                services.
            </p>
            <p class="prod-text">
                Weekly habit package - 4 Lessons per month at $159. (One lesson
                per week at the client’s preferred time &amp; choosing).
            </p>
            <p class="prod-text">
                Monthly freedom package - 5 lessons per month at $199. (All
                Lessons distributed based on client’s preferences over a 30-day
                period).
            </p>
            <p class="prod-text">
                Monthly packages include progress reports. These reports are
                feedback from the teachers regarding student’s progress and
                areas of required attention as well as recommendations or
                suggestions for academic and learning enhancement.
            </p>
        </label>
    </div>
</div>

<style>
    @import url(https://fonts.googleapis.com/css?family=Lato);

    @import url(https://fonts.googleapis.com/css?family=Open+Sans);

    .section h1 {
        text-align: center;
        display: block;
        margin: 20px auto;
        max-width: 1080px;
    }

    .prod-heading {
        font-family: Lato;
        font-weight: 400;
        font-size: 19px;
        -webkit-transition: text-indent 0.2s;
        text-indent: 20px;
        color: #333;
    }

    .prod-text {
        font-family: Open Sans;
        font-weight: 400;
        color: #919191;
        width: 95%;
        padding-left: 20px;
        margin-bottom: 30px;
    }

    .prod {
        width: 1000px;
        margin: 0 auto;
        background: white;
        border-radius: 4px;
        position: relative;
        border: 1px solid #e1e1e1;
        /* padding-bottom: 2em; */
    }
    .prod label {
        display: block;
        position: relative;
        overflow: hidden;
        cursor: pointer;
        height: 56px;
        padding-top: 1px;
        background-color: #fafafa;
        border-bottom: 1px solid #e1e1e1;
    }

    .prod input[type="checkbox"] {
        display: none;
    }

    .prod .prod-arrow {
        width: 5px;
        height: 5px;
        transition: -webkit-transform 0.8s;
        transition: transform 0.8s;
        transition: transform 0.8s, -webkit-transform 0.8s;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
        border-top: 2px solid #42a5ff;
        border-right: 2px solid #42a5ff;
        float: right;
        position: relative;
        top: -30px;
        right: 27px;
        -webkit-transform: rotate(45deg);
        transform: rotate(45deg);
    }

    .prod input[type="checkbox"]:checked + label > .prod-arrow {
        transition: -webkit-transform 0.8s;
        transition: transform 0.8s;
        transition: transform 0.8s, -webkit-transform 0.8s;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
        -webkit-transform: rotate(135deg);
        transform: rotate(135deg);
    }
    .prod input[type="checkbox"]:checked + label {
        display: block;
        background: rgba(255, 255, 255, 255) !important;
        color: #4f7351;
        height: 225px;
        transition: height 0.8s;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
    }

    .prod input[id="prod-a"][type="checkbox"]:checked + label {
        display: block;
        background: rgba(255, 255, 255, 255) !important;
        color: #4f7351;
        height: 375px;
        transition: height 0.8s;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
    }

    .prod input[id="prod-c"][type="checkbox"]:checked + label {
        display: block;
        background: rgba(255, 255, 255, 255) !important;
        color: #4f7351;
        height: 315px;
        transition: height 0.8s;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
    }
    .prod input[id="prod-d"][type="checkbox"]:checked + label {
        display: block;
        background: rgba(255, 255, 255, 255) !important;
        color: #4f7351;
        height: 650px;
        transition: height 0.8s;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
    }

    .prod input[id="prod-e"][type="checkbox"]:checked + label {
        display: block;
        background: rgba(255, 255, 255, 255) !important;
        color: #4f7351;
        height: 125px;
        transition: height 0.8s;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
    }

    .prod input[id="prod-f"][type="checkbox"]:checked + label {
        display: block;
        background: rgba(255, 255, 255, 255) !important;
        color: #4f7351;
        height: 325px;
        transition: height 0.8s;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
    }

    .prod input[type="checkbox"]:not(:checked) + label {
        display: block;
        transition: height 0.8s;
        height: 60px;
        -webkit-transition-timing-function: cubic-bezier(
            0.68,
            -0.55,
            0.265,
            1.55
        );
    }

    ::-webkit-scrollbar {
        display: none;
    }
</style>
