<script>
    let count = 0
    const onClick = () => {
        count++
    }
</script>

<section>
    <h1>Counter: {count}</h1>
</section>
<section>
    <button on:click={onClick}>
        Click
    </button>
</section>
