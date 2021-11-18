<script>
    export let charities;
</script>

<div>
    <h2>Charity List</h2>
    {#if charities !== undefined}
    <pre>{charities}</pre>
    <ul>
        {#each charities as charity}
        <li>{charity.title} - {charity.category}</li>
        {/each}
    </ul>
    {:else} 
        <p>Data belum tersedia</p>
    {/if}
</div>