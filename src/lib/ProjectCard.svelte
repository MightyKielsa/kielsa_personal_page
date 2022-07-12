<script>
	import Card, { Actions, Content } from '@smui/card';
	import Button, { Label } from '@smui/button';
	//import IconButton, { Icon } from '@smui/icon-button';

	function onClick() {
		return;
	}
</script>

<main>
	<div class="card-container">
		<Card>
			<Content>A card with a full-bleed action.</Content>
			<Actions fullBleed>
				<Button on:click={() => clicked++}>
					<Label>Action</Label>
					<i class="material-icons" aria-hidden="true">arrow_forward</i>
				</Button>
			</Actions>
		</Card>
	</div>
</main>

<style>
</style>
