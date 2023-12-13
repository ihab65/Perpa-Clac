<script>
    export let name;
    let cc = 0;
    let ds = 0;
    let es = 0;
    let tp = 0;
</script>

<div class="card">

    <p class="label">{name}</p>
    <p class="label">cc</p>
    <input class="intake" type="number" max=20 min=0 bind:value={cc} />
    <p class="label">ds</p>
    <input class="intake" type="number" max=20 min=0 bind:value={ds} />
    <p class="label">es</p>
    <input class="intake" type="number" max=20 min=0 bind:value={es} />
    <p class="label">tp</p>
    <input class="intake" type="number" max=20 min=0 bind:value={tp} />

    <p>{(ds*0.2+cc*0.1+es*0.5+tp*0.2).toFixed(2)}</p>
</div>

<style>
    .card {
        display: flex;
        flex-flow: row wrap;
        align-items: center;
    }
    .label {
        margin: 5px 10px 5px 0;
    }
    .intake {
        vertical-align: middle;
        margin: 5px 10px 5px 0;
        padding: 10px;
        background-color: #000;
        border: 1px solid #ddd;
        width: 100px;
    }
</style>