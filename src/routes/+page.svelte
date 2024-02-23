<script>
	import Project from '../components/Project.svelte';

	const base_url = "https://martintm.dev";
</script>

<h1 class="title">Some of my stuff</h1>

<div class="projects">
	<Project
	image_url="/projects/brainfuck.png"
	title="Brainfuck Interpreter"
	link={base_url + "/brainfuck"}>
	Simple online interpreter for the esoteric language <a href="https://en.wikipedia.org/wiki/Brainfuck" target="_blank">Brainfuck</a></Project>

	<Project
	image_url="/projects/flo-stats.png"
	title="FloWrestling Stats"
	link={base_url + "/flo-stats"}
	description="A tool to calculate wrestling statistics like your win-to-loss ratio" />

	<Project
	image_url="/projects/snake.png"
	title="Snake"
	link={base_url + "/snake"}
	description="Simple snake game (I was bored)" />
</div>

<style>
	* {
		text-align: left;
		margin: 0;
	}
	
	.title {
		margin-top: 10px;
		margin-bottom: 10px;
	}

	.projects {
		display: flex;
		flex-wrap: wrap;
		gap: 20px;
	}

	/*:global(.projects > *) {
		flex-grow: 0;
		flex-shrink: 1;
		flex-basis: 40%;
	}*/
</style>