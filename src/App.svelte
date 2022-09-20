<script>
    import Counter from './lib/Counter.svelte'
    import Agility from "./lib/Agility.svelte";
    // import ToDo from "./lib/ToDo.svelte";
    let visibleComponent = 'Simple'
</script>

<header>
    <button on:click={() => visibleComponent = 'Counter'}>Counter</button>
    <button on:click={() => visibleComponent = 'Agility'}>Agility</button>
</header>
<section>
    {#if visibleComponent === 'Counter'}
        <Counter/>
    {:else if visibleComponent === 'Agility'}
        <Agility/>
    {/if}
</section>

