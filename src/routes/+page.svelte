<script>
	import Project from '../components/Project.svelte';
	import Footer from '../components/Footer.svelte';

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

	<Project
	image_url={base_url + "/game-of-life/favicon.svg"}
	title="Conway's Game of Life"
	link={base_url + "/game-of-life"}>
	A cellular automation created by <a href="https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life" target="_blank">John Horton Conway</a>
	</Project>

	<Project
	image_url={base_url + "/random-math-game/favicon.png"}
	title="Random Math Game"
	link={base_url + "/random-math-game"}
	description="A board game one of my math teachers showed me" />

	<Project
	image_url="/projects/flappy-bird-ai.png"
	title="Flappy Bird AI"
	link={base_url + "/flappy-bird-ai"}
	description="Neural network trains itself to play Flappy Bird" />
</div>

<Footer />

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
