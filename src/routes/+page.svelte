<script>
	import {
		Button,
		Typography,
		Row,
		Column,
		Card,
		Alert,
		Container,
		Badge
	} from '$lib';

	function onClickButton() {
		alert('Clicked button');
	}
</script>

<Container size='lg'>
	<Typography variant='h1' weight='1000'>Sun UI &#127774;</Typography>
	
	<Row classes="mb-5">
		<Column>
			<Typography variant='h3'>Typography!</Typography>
		</Column>
	</Row>
	
	<h3>Buttons</h3>
	<Row classes="mb-5" justify='space-evenly'>
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
			<Button on:click={() => alert('Hello')} color='success'>Success</Button>
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

	<Row>
		<Column col={6}>
			<div class="bg-tertiary text-center">
				Growing column
			</div>
		</Column>
	</Row>
	
	<Typography variant="h3" classes="mt-5">Cards</Typography>
	<Row>
		<Column xs={3}>
			<Card>
				<Typography variant="h4">Card 1</Typography>
				<Typography variant="p">Card content!</Typography>
			</Card>
		</Column>
		<Column xs={6}>
			<Card>
				<Typography variant="h4">Card 2</Typography>
				<Typography variant="p">Card content!</Typography>
			</Card>
		</Column>
		<Column xs={3}>
			<Card>
				<Typography variant="h4">Card 2</Typography>
				<Typography variant="p">Card content!</Typography>
			</Card>
		</Column>
	</Row>
	
	<Typography variant="h3" classes="mt-5">Alerts</Typography>
	<Alert color="primary">Primary</Alert>
	<Alert color="secondary">Secondary</Alert>
	<Alert color="tertiary">Tertiary</Alert>
	<Alert color="success">Success</Alert>
	<Alert color="warning">Warning</Alert>
	<Alert color="danger">Danger</Alert>
	<Alert color="info">Info</Alert>

	<Typography variant="h3" classes="mt-5">Badges</Typography>
	<Row align='center'>
		<Column>
			<Button color='primary'>
				Profile
				<Badge color='light'>5</Badge>
			</Button>
		</Column>
		<Column>
			<Badge color='primary'>Primary</Badge>
		</Column>
		<Column>
			<Badge color='secondary'>Secondary</Badge>
		</Column>
		<Column>
			<Badge color='success'>Success</Badge>
		</Column>
		<Column>
			<Badge color='warning'>Warning</Badge>
		</Column>
		<Column>
			<Badge color='danger'>Danger</Badge>
		</Column>
		<Column>
			<Badge color='light'>Light</Badge>
		</Column>
		<Column>
			<Badge color='dark'>Dark</Badge>
		</Column>
	</Row>

</Container>
