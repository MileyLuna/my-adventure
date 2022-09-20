<script>
	import About from "./About.svelte";
	import Experience from "./Experience.svelte";
	import Project from "./Project.svelte";

	let showAbout = false;
	let showExp = false;
	let showPro = false;

	let toggleAbout = () => {
		showAbout = !showAbout;
	};

	let toggleExp = () => {
		showExp = !showExp;
	};

	let togglePro = () => {
		showPro = !showPro;
	};
</script>

<!-- <About {showAbout} on:click={toggleAbout} />
<Experience {showExp} on:click={toggleExp} />
<Project {showPro} on:click={togglePro} /> -->
<main>
	<!-- <div on:click={toggleAbout} class="blank">about me</div>
	<br />
	<div on:click={toggleExp} class="blank">experience</div>
	<br />
	<div on:click={togglePro} class="blank">projects</div> -->

	<div id="tab0" />
	<div id="tab1" />
	<div id="tab2" />
	<div id="tab3">
		<About />
	</div>
	<div id="tab4" class="title">
		<h1>Miley Vang</h1>
		<p>Software Developer</p>
	</div>
</main>

<style>

	#tab0,
	#tab1,
	#tab2,
	#tab3,
	#tab4 {
		height: 100%;
		position: absolute;
		box-shadow: 6px 0px 6px rgba(0, 0, 0, 0.3);
		transition: all 0.5s ease;
	}

	#tab0:hover ~ div,
	#tab1:hover ~ div,
	#tab2:hover ~ div,
	#tab3:hover ~ div {
		transform: translateX(-80vw);
	}
	#tab0 {
		width: 100vw;
		background: black;
	}
	#tab1 {
		width: 95vw;
		background: #31152b;
	}
	#tab1::after {
		content: "";
		position: absolute;
		width: 5vw;
		height: 25vh;
		background: #31152b;
		border-radius: 0 20px 20px 0;
		top: 75%;
		right: -4vw;
	}
	#tab2 {
		width: 90vw;
		background: #723147;
	}
	#tab2::after {
		content: "";
		position: absolute;
		width: 5vw;
		height: 25vh;
		background: #723147;
		border-radius: 0 20px 20px 0;
		top: 50%;
		right: -4vw;
	}
	#tab3 {
		width: 85vw;
		background: #cc4452;
	}
	#tab3::after {
		content: "";
		position: absolute;
		width: 5vw;
		height: 25vh;
		background: #cc4452;
		border-radius: 0 20px 20px 0;
		top: 25%;
		right: -4vw;
	}
	#tab4 {
		width: 80vw;
		background: #e6b098;
	}
	#tab4::after {
		content: "";
		position: absolute;
		width: 5vw;
		height: 25vh;
		background: #e6b098;
		border-radius: 0 20px 20px 0;
		top: 0;
		right: -4vw;
	}

	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	.title {
		font-family: "Cairo";
		text-align: center;
		color: #fff;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		height: 100vh;
		letter-spacing: 1px;
		line-height: 2;
	}

	h1 {
		background-image: url(https://media.giphy.com/media/26BROrSHlmyzzHf3i/giphy.gif);
		background-size: cover;
		color: transparent;
		-moz-background-clip: text;
		-webkit-background-clip: text;
		text-transform: uppercase;
		font-size: 120px;
		margin: 0px 0;
	}
</style>
