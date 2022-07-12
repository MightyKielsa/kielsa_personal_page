<script>
	export let skillObj;
</script>

<main>
	<img src={skillObj.imgUrl} alt={skillObj.imgAlt} />
	<h3>{skillObj.header}</h3>
	<p>{skillObj.text}</p>
</main>

<style>
	img {
		width: 10vw;
		height: auto;
	}
</style>
