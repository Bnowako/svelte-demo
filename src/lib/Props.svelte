<script>
    import Nested from "./Nested.svelte";
    let fromParent = 'default'

</script>

<div>
    <Nested {fromParent} />
    <input type="text" bind:value={fromParent}/>
</div>
