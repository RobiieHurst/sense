<script>
    import Particles from "svelte-particles";
	import { loadFull } from "tsparticles";

    let particlesConfig = {
		fullScreen: { enable: false },
		particles: {
			number: {
				value: 80,
				density: {
					enable: true,
					value_area: 800,
				},
			},
			color: {
				value: "#fff",
			},
			shape: {
				type: "circle",
				stroke: {
					width: 0,
					color: "#000000",
				},
				polygon: {
					nb_sides: 5,
				},
				image: {
					src: "img/github.svg",
					width: 100,
					height: 100,
				},
			},
			opacity: {
				value: 0.5,
				random: false,
				anim: {
					enable: false,
					speed: 1,
					opacity_min: 0.1,
					sync: false,
				},
			},
			size: {
				value: 3,
				random: true,
				anim: {
					enable: false,
					speed: 40,
					size_min: 0.1,
					sync: false,
				},
			},
			line_linked: {
				enable: true,
				distance: 150,
				color: "#fff",
				opacity: 0.4,
				width: 1,
			},
			move: {
				enable: true,
				speed: 6,
				direction: "none",
				random: false,
				straight: false,
				out_mode: "out",
				bounce: false,
				attract: {
					enable: false,
					rotateX: 600,
					rotateY: 1200,
				},
			},
		},
		interactivity: {
			detect_on: "window",
			events: {
				onhover: {
					enable: true,
					mode: "grab",
				},
				onclick: {
					enable: true,
					mode: "push",
				},
				resize: true,
			},
			modes: {
				grab: {
					distance: 400,
					line_linked: {
						opacity: 1,
					},
				},
				bubble: {
					distance: 400,
					size: 40,
					duration: 2,
					opacity: 8,
					speed: 3,
				},
				repulse: {
					distance: 200,
					duration: 0.4,
				},
				push: {
					particles_nb: 4,
				},
				remove: {
					particles_nb: 2,
				},
			},
		},
		retina_detect: true,
	};

	let onParticlesLoaded = (event) => {
		const particlesContainer = event.detail.particles;

		// you can use particlesContainer to call all the Container class
		// (from the core library) methods like play, pause, refresh, start, stop
	};

	let particlesInit = async (engine) => {
		// you can use main to customize the tsParticles instance adding presets or custom shapes
		// this loads the tsparticles package bundle, it's the easiest method for getting everything ready
		// starting from v2 you can add only the features you need reducing the bundle size
		await loadFull(engine);
	};
</script>

<div class="hero">
    <h1>Metaverse<span>- M&G Tutoring -</span></h1>
	<div id="tsparticles">
		<Particles
			id="tsparticles"
			options={particlesConfig}
			on:particlesLoaded={onParticlesLoaded}
			{particlesInit}
		/>
	</div>
</div>

<style>
	@import url(https://fonts.googleapis.com/css?family=Open+Sans:600,300);

	.hero {
		height: 20vh;
		position: relative;
	}

	#tsparticles {
		width: 100%;
		height: 100%;
        z-index: -1;
		background-color: #42a5ff;
	}

	h1 {
		position: absolute;
		top: 10%;
		left: 50%;
		transform: translate(-50%, -50%);
		color: #FFF;
		font: normal 600 72px/1 "Open Sans", sans-serif;
		text-align: center;
	}
	h1 span {
		display: block;
		font-size: 40px;
		font-weight: 300;
	}

</style>