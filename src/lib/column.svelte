<script>
	export let gap = 1;
	export let classes = '';
	export let xs;
	export let sm;
	export let md;
	export let lg;
	export let xl;
	export let xxl;
	let colClasses = '';
	$: {
		if (xs)
			colClasses += `col-xs-${xs} `;
		if (sm)
			colClasses += `col-sm-${sm} `;
		if (md)
			colClasses += `col-md-${md} `;
		if (lg)
			colClasses += `col-lg-${lg} `;
		if (xl)
			colClasses += `col-xl-${xl} `;
		if (xxl)
			colClasses += `col-xxl-${xxl} `;

		if (colClasses.length == 0)
		{
			colClasses = 'col-auto';
		}
	}
</script>

<div
	class="{colClasses} {classes}"
>
	<slot />
</div>

