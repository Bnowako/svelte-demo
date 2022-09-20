<script>
    let agility = 0;
    let power = 0;

    function incrementAgility() {
        agility++;
    }

    function incrementPower() {
        power++;
    }

    function incrementPowerAndAgility() {
        agility += 5;
        power += 7;
    }
</script>
<div>
<section>
Agility: {agility}
Power: {power}
Stats: {agility * power}
</section>
<p>
    <button on:click={incrementAgility}>+ Agility</button>
    <button on:click={incrementPower}>+ Power</button>
    <button on:click={incrementPowerAndAgility}>Level Up</button>
</p>
</div>
