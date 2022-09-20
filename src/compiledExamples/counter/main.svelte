<script>
	let count = 0
	const onClick = () => {
		count++
	}
</script>
<p>Counter: {count}</p>
<button on:click={onClick}>
	Click
</button>
