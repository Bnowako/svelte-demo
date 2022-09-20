<script>
	let agility = 0;
	let power = 0;
	function incrementAgility() {
		agility ++;
	}
	function incrementPower() {
		power ++;
	}
	function levelUp() {
		agility += 5;
		power += 7;
	}
</script>
Agility: {agility}
Power: {power}
Stats: {agility * power}
<button on:click={incrementAgility}>+ Agility</button>
<button on:click={incrementPower}>+ Power</button>
<button on:click={levelUp}>Level Up</button>
