<script>
	import {
		Button,
		Typography,
		Row,
		Column,
		Card
	} from '$lib';

	function onClickButton() {
		alert('Clicked button');
	}
</script>

<Typography variant='h1' weight='1000'>Sun UI &#127774;</Typography>

<Row classes="mb-5">
	<Column>
		<Typography variant='h3'>Typography!</Typography>
	</Column>
</Row>

<h3>Buttons</h3>
<Row classes="mb-5" justify='space-evenly'>
	<Column>
		<Button on:click={() => alert('Hello')} />
	</Column>
	<Column>
		<Button on:click={() => alert('Hello')} color='primary'>Primary</Button>
	</Column>
	<Column>
		<Button on:click={() => alert('Hello')} color='secondary'>Secondary</Button>
	</Column>
	<Column>
		<Button on:click={() => alert('Hello')} color='tertiary'>Tertiary</Button>
	</Column>
	<Column>
		<Button on:click={() => alert('Hello')} color='info'>Info</Button>
	</Column>
	<Column>
		<Button on:click={() => alert('Hello')} color='danger'>&#128293;</Button>
	</Column>
	<Column>
		<Button on:click={() => alert('Hello')} color='warning'>Warning</Button>
	</Column>
</Row>

<h3>Grid system</h3>
<Row>
	<Column xs={12}>
		<div class="bg-tertiary text-center">
			xs-12
		</div>
	</Column>
</Row>

<Row>
	<Column xs={6}>
		<div class="bg-tertiary text-center">
			xs-6
		</div>
	</Column>
	<Column xs={6}>
		<div class="bg-tertiary text-center">
			xs-6
		</div>
	</Column>
</Row>

<Row>
	<Column xs={6} md={4} lg={3} xl={12} xxl={4}>
		<div class="bg-tertiary text-center">
			Column
		</div>
	</Column>
	<Column xs={6} md={4} lg={3} xl={2} xxl={8}>
		<div class="bg-tertiary text-center">
			Column
		</div>
	</Column>
	<Column xs={4} md={4} lg={3} xl={2} xxl={12}>
		<div class="bg-tertiary text-center">
			Column
		</div>
	</Column>
	<Column xs={4} md={6} lg={3} xl={2} xxl={4}>
		<div class="bg-tertiary text-center">
			Column
		</div>
	</Column>
	<Column xs={4} md={6} lg={12} xl={2} xxl={4}>
		<div class="bg-tertiary text-center">
			Column
		</div>
	</Column>
	<Column xs={12} md={6} lg={6} xl={2} xxl={4}>
		<div class="bg-tertiary text-center">
			Column
		</div>
	</Column>
	<Column xs={12} md={6} lg={6} xl={2} xxl={12}>
		<div class="bg-tertiary text-center">
			Column
		</div>
	</Column>
</Row>

<Typography variant="h3" classes="mt-5">Cards</Typography>
<Card>
	<Typography variant="h4">Hello</Typography>
	<Typography variant="p">Card content!</Typography>
</Card>
