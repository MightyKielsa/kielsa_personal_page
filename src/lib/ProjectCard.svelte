<script>
	import Card, { Actions, Content } from '@smui/card';
	import Button, { Label } from '@smui/button';
	//import IconButton, { Icon } from '@smui/icon-button';
	export let projectObj;

	function onClick() {
		return;
	}
</script>

<main>
	<div class="card-container">
		<Card class="card-class">
			<img src={projectObj.imgSrc} alt={projectObj.imgAlt} />
			<div class="text-container">
				<h3>{projectObj.projectTitle}</h3>
				<Content>{projectObj.projectDescription}</Content>
			</div>
			<Actions fullBleed>
				<div class="button-div">
					<Button on:click={onClick} variant="unelevated">
						<Label>View Project</Label>
						<i class="material-icons" aria-hidden="true">arrow_forward</i>
					</Button>
				</div>
			</Actions>
		</Card>
	</div>
</main>

<style>
	.card-container {
		max-width: 300px;
		box-shadow: 5px 5px 10px 2px rgba(0, 0, 0, 0.8);
		border-radius: 3%;
		height: auto;
	}
	.card-class {
		background-color: #ffc107;
	}
	.text-container {
		display: flex;
		flex-direction: column;
		height: 15vh;
	}

	h3 {
		text-align: center;
	}
	img {
		border-radius: 3%;
		width: 10vw;
		height: auto;
		margin-left: auto;
		margin-right: auto;
		margin-top: 10%;
	}
	.button-div {
		width: 50%;
		margin: 2vh auto 2vh auto;
	}
</style>
