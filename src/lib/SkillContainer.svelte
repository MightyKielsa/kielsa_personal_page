<script>
	import Skill from './Skill.svelte';
	let skillArr = [
		{
			imgUrl:
				'https://yt3.ggpht.com/a-/AAuE7mAjCgbd8Wq35r6JNQr0xXzJZsZThycm7ayRFw=s900-mo-c-c0xffffffff-rj-k-no',
			imgAlt: 'A pic of a bird',
			header: 'Image 1',
			text: 'dsadj;dfklsfkh dfsa asljkfh'
		},
		{
			imgUrl:
				'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.TCK8iqPQ5jztcDNWEANeVQHaHa%26pid%3DApi&f=1',
			imgAlt: 'A powerful meme',
			header: 'Image 2',
			text: 'fdagdfgshgfhfh fdhf jgf fgh'
		},
		{
			imgUrl:
				'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.redd.it%2F7hplh03z2lf01.png&f=1&nofb=1',
			imgAlt: 'A random flag',
			header: 'Image 3',
			text: 'Itchy bum tadum tadum'
		}
	];
</script>

<main>
	<div>
		{#each skillArr as skillObj}
			<Skill {skillObj} />
		{/each}
	</div>
</main>

<style>
	div {
		display: flex;
		flex-direction: column;
		width: 50%;
	}
</style>
