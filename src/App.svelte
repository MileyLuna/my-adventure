<script>
	import About from "./About.svelte";
	import Experience from "./Experience.svelte";
	import Project from "./Project.svelte";
	import Contact from "./Contact.svelte";


</script>

<main>
	<div id="tab0">
		<Contact />
	</div>
	<div id="tab1">
		<Project />
	</div>
	<div id="tab2">
		<!-- <Experience /> -->
	</div>
	<div id="tab3">
		<About />
	</div>
	<div id="tab4" class="title">
		<h1>Miley Vang</h1>
		<p>Software Developer | Tech Mom | First Generation | Foodie</p>
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
		background: #000000;
	}
	#tab1 {
		width: 95vw;
		background: #2a0001;
	}
	#tab1::after {
		content: "PROJECTS";
		position: absolute;
		width: 5vw;
		height: 20vh;
		background: #2a0001;
		border-radius: 0 20px 20px 0;
		top: 75%;
		right: -4vw;
		padding: 20px 10px 20px 20px;
		writing-mode: vertical-rl;
		text-orientation: mixed;
		font-size: 1.25em;

	}
	#tab2 {
		width: 90vw;
		background: #450000;
	}
	#tab2::after {
		content: "EXPERIENCES";
		position: absolute;
		width: 5vw;
		height: 25vh;
		background: #450000;
		border-radius: 0 20px 20px 0;
		top: 50%;
		right: -4vw;
		padding: 20px 10px 20px 20px;
		writing-mode: vertical-rl;
		text-orientation: mixed;
		font-size: 1.25em;


	}
	#tab3 {
		width: 85vw;
		background: #620000;

		
	}
	#tab3::after {
		content: "JOURNEY";
		position: absolute;
		width: 5vw;
		height: 25vh;
		background: #620000;
		border-radius: 0 20px 20px 0;
		top: 25%;
		right: -4vw;
		padding: 20px 10px 20px 20px;
		writing-mode: vertical-rl;
		text-orientation: mixed;
		font-size: 1.25em;
	}
	#tab4 {
		width: 80vw;
		background: #740303;
	}
	#tab4::after {
		content: "";
		position: absolute;
		width: 5vw;
		height: 25vh;
		background: #740303;
		border-radius: 0 20px 20px 0;
		top: 0;
		right: -4vw;
		
	}

	main {
		text-align: center;
		/* padding: 1em; */
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
		background-image: url(https://media4.giphy.com/media/26BROrSHlmyzzHf3i/giphy.gif?cid=790b761183d2fb0a0b37bb106da3228b203230b21214ab3b&rid=giphy.gif&ct=g);
		background-size: 200px;
		color: transparent;
		-moz-background-clip: text;
		-webkit-background-clip: text;
		text-transform: uppercase;
		font-size: 120px;
		margin: 0px 0;
	}
</style>
