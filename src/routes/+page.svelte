<script>
	import { Button, Typography } from '$lib';

	function onClickButton() {
		alert('Clicked button');
	}
</script>

<Typography variant='h1' weight='1000'>Sun UI &#127774;</Typography>

<Typography variant='h3'>Typography!</Typography>

<h3>Buttons</h3>
<Button on:click={() => alert('Hello')} />
<Button on:click={() => alert('Hello')} color='primary'>Primary</Button>
<Button on:click={() => alert('Hello')} color='secondary'>Secondary</Button>
<Button on:click={() => alert('Hello')} color='tertiary'>Tertiary</Button>
<Button on:click={() => alert('Hello')} color='danger'>&#128293;</Button>
<Button on:click={() => alert('Hello')} color='warning'>Warning</Button>
