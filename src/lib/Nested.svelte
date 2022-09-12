<script>
    export let fromParent
</script>

<div>
    <p>Props from parent: {fromParent}</p>
    <button on:click={() => fromParent = fromParent + 'AddedValue'}>Add </button>
</div>
