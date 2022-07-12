<script>
	import SkillContainer from '../lib/SkillContainer.svelte';
	import ProjectCard from '../lib/ProjectCard.svelte';

	let projectsArr = [
		{
			imgSrc: '/project1-pic.jpg',
			imgAlt: 'A laptop, smartphone and notebook lying on a desk',
			projectTitle: 'ONE WEEK PROJECT',
			projectDescription:
				"A 'Bootcamper Helper app made during my time at School of code, the timeframe for the project was 5 days"
		},
		{
			imgSrc: '/project2-pic.jpg',
			imgAlt: 'A screen displaying computer code',
			projectTitle: 'FOUR WEEK PROJECT',
			projectDescription:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
		},
		{
			imgSrc: '/project3-pic.jpg',
			imgAlt: 'A personal computer screen displaying a futuristic app',
			projectTitle: 'TOTALLY LEGIT PROJECT',
			projectDescription:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
		}
	];
</script>

<main>
	<SkillContainer />
	<div class="projects-row">
		{#each projectsArr as project}
			<ProjectCard projectObj={project} />
		{/each}
	</div>
</main>

<style>
	main {
		height: 300vh;
	}
	.projects-row {
		display: flex;
		justify-content: space-around;
		height: 50vh;
	}
</style>
