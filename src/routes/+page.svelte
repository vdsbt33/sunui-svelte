<script>
	import { Button, Typography, Row, Column } from '$lib';

	function onClickButton() {
		alert('Clicked button');
	}
</script>

<Typography variant='h1' weight='1000'>Sun UI &#127774;</Typography>

<Typography variant='h3'>Typography!</Typography>

<h3>Buttons</h3>
<Row>
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
		<Button on:click={() => alert('Hello')} color='danger'>&#128293;</Button>
	</Column>
	<Column>
		<Button on:click={() => alert('Hello')} color='warning'>Warning</Button>
	</Column>
</Row>

<h3>Grid system</h3>
<Row>
	<Column xs={12} classes="bg-secondary text-center">
		xs-12
	</Column>
</Row>

<hr />

<Row>
	<Column xs={6} classes="bg-secondary text-center">
		xs-6
	</Column>
	<Column xs={6} classes="bg-secondary text-center">
		xs-6
	</Column>
</Row>

<hr />

<Row>
	<Column xs={6} md={4} lg={3} xl={12} xxl={4} classes="bg-secondary text-center">
		Column
	</Column>
	<Column xs={6} md={4} lg={3} xl={2} xxl={8} classes="bg-secondary text-center">
		Column
	</Column>
	<Column xs={4} md={4} lg={3} xl={2} xxl={12} classes="bg-secondary text-center">
		Column
	</Column>
	<Column xs={4} md={6} lg={3} xl={2} xxl={4} classes="bg-secondary text-center">
		Column
	</Column>
	<Column xs={4} md={6} lg={12} xl={2} xxl={4} classes="bg-secondary text-center">
		Column
	</Column>
	<Column xs={12} md={6} lg={6} xl={2} xxl={4} classes="bg-secondary text-center">
		Column
	</Column>
	<Column xs={12} md={6} lg={6} xl={2} xxl={12} classes="bg-secondary text-center">
		Column
	</Column>
</Row>
