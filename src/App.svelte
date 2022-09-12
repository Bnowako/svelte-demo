<script>
    import Counter from './lib/Counter.svelte'
    import SimpleComponent from "./lib/SimpleComponent.svelte";
    import ReactiveComponent from "./lib/ReactiveComponent.svelte";
    import Props from "./lib/Props.svelte";

    let visibleComponent = 'Simple'
</script>

{#if visibleComponent === 'Counter'}
    <Counter/>
{:else if visibleComponent === 'Simple'}
    <SimpleComponent/>
{:else if visibleComponent === 'Reactive'}
    <ReactiveComponent/>
{:else if visibleComponent === 'Props'}
    <Props/>
{:else if visibleComponent === 'Binding'}
{:else if visibleComponent === 'If'}
{:else if visibleComponent === 'Else'}

{/if}

<div class="my-4">
    <button on:click={() => visibleComponent = 'Simple'}>Simple</button>
    <button on:click={() => visibleComponent = 'Counter'}>Counter</button>
    <button on:click={() => visibleComponent = 'Reactive'}>Reactive</button>
    <button on:click={() => visibleComponent = 'Props'}>Props</button>
</div>
