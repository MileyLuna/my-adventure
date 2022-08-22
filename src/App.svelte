<script>
	import About from "./About.svelte";
	import Experience from "./Experience.svelte";
	import Project from './Project.svelte';

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

<About {showAbout} on:click={toggleAbout} />
<Experience {showExp} on:click={toggleExp}/>
<Project {showPro} on:click={togglePro}/>
<main>
	<div on:click={toggleAbout} class='blank'>about me</div>
	<br>
	<div on:click={toggleExp} class='blank'>experience</div>
	<br>
	<div on:click={togglePro} class='blank'>projects</div>

	<div class="title">
		<h1 >Miley Vang</h1>
		<p>Software Developer</p>

	</div>
</main>



<style>
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
	color: #FFF;
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	height: 100vh;
	letter-spacing: 1px;
	line-height:2
}

h1 {
	background-image: url(https://media.giphy.com/media/26BROrSHlmyzzHf3i/giphy.gif);
	background-size: cover;
	color: transparent;
	-moz-background-clip: text;
	-webkit-background-clip: text;
	text-transform: uppercase;
	font-size: 120px;
	margin: 10px 0;
}



</style>
