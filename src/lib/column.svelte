<script>
	export let classes = '';
	export let col;
	export let xs;
	export let sm;
	export let md;
	export let lg;
	export let xl;
	export let xxl;
	let addClasses = '';
	$: {
		let classArray = []

		if (col)
		{
			classArray.push(`col-${col}`);
		}
		else
		{
			if (xs)
				classArray.push(`col-xs-${xs}`);
			if (sm)
				classArray.push(`col-sm-${sm}`);
			if (md)
				classArray.push(`col-md-${md}`);
			if (lg)
				classArray.push(`col-lg-${lg}`);
			if (xl)
				classArray.push(`col-xl-${xl}`);
			if (xxl)
				classArray.push(`col-xxl-${xxl}`);
	
			if (classArray.length == 0)
				classArray.push('col-auto');
		}

		addClasses = classArray.join(' ');
	}
</script>

<div
	class="{addClasses} {classes}"
>
	<slot />
</div>

<style>
	div {
		box-sizing: border-box;
		padding: .25rem;
	}
</style>

