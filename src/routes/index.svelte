<script>
    import Hero from "$lib/hero.svelte";
    import { fly } from "svelte/transition";
</script>

<Hero />

<div class="vision">
    <h1>Vision</h1>
    <div class="row">
        <div class="column">
            <p>
                Education in all its forms is one of the most profoundly
                important experiences of every person's life. It can represent
                the most direct manifestation of our progress in life and as
                such it deserves consistent consideration and reflection.
            </p>
            <p>
                At SENSE, we believe that underpinning all effective education
                are the values of growth, excitement and faith in the wisdom and
                inalienable truths that bind our collective human experiences.
                We believe that each student, family and organization should
                have the freedom to choose an education that will result in the
                perpetual betterment of both the individual and their chosen
                society. Let learning make sense.
            </p>
            <br />
        </div>
        <div class="column">
            <img
                in:fly={{ x: 200, duration: 2000 }}
                src="/child_learning_2.jpg"
                width="400px"
                alt="vision img"
            />
            <img
                in:fly={{ y: 200, duration: 2000 }}
                src="/learning_making_sense.jpg"
                width="400px"
                alt="vision img"
            />
        </div>
    </div>
</div>

<div class="mission_outer">
    <div class="mission">
        <h1>Mission</h1>

        <div class="row">
            <div class="column">
                <p>
                    With the appropriate transfer of information and
                    instruction, what and how we learn can help shape our
                    destiny for success and lifelong satisfaction. At SENSE we
                    believe that all information achieves its true power once it
                    is accessible, understandable and engaging to those that
                    seek it.
                </p>
                <br />
                <p>
                    Our vision is to create an enterprise that focuses on
                    providing the means and methods for effective information
                    absorption within every element of our lives from personal
                    curiosity and having the desire to learn a new skill or idea
                    to schooling, professional upskilling and holistic workplace
                    training. SENSE envisions creating a system where any
                    person’s desire for personal and/or professional upliftment
                    can be achieved through the fusion of pragmatic knowledge
                    with sensational teaching methods.
                </p>
            </div>
            <div class="column">
                <img
                    in:fly={{ x: 200, duration: 2000 }}
                    src="/child_learning.jpg"
                    width="400px"
                    alt="vision img"
                />
            </div>
        </div>

        <br />
    </div>
</div>

<style>
    .vision {
        text-align: center;
        display: block;
        max-width: 1080px;
        margin: 50px auto;
    }

    .vision p {
        text-align: left;
    }

    .vision h1 {
        color: black;
    }

    .vision img {
        border-radius: 15%;
    }

    .mission_outer {
        background-color: #42a5ff;
    }

    .mission {
        text-align: center;
        display: block;
        margin: 50px auto;
        max-width: 1080px;
    }

    .mission p {
        text-align: left;
    }

    .mission p,
    h1 {
        color: #fff;
    }

    .mission img {
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
