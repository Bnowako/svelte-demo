<script>
    let salary = 0
    $: salaryGross = salary - tax
    $: tax = salary * 0.1
</script>

<div>
    <p>Tax: {tax}</p>
    <p>SalaryGross: {salaryGross}</p>
    <input type="number" bind:value={salary}>
</div>
