<script>
    export let cc = 0;
    export let ds = 0;
    export let es = 0;
    export let tp = 0;
</script>
<p>cc</p><br>
<input class="intake" type="number" bind:value={cc} />
<p>ds</p>
<input class="intake" type="number" bind:value={ds} />
<p>es</p>
<input class="intake" type="number" bind:value={es} />
<p>tp</p>
<input class="intake" type="number" bind:value={tp} />

<p>{ds*0.2+cc*0.1+es*0.5+tp*0.2}</p>

<style>
    .intake {
        
    }
</style>