<!-- src/components/Cards.svelte -->
<script>
    export let title;
    export let description;
    export let imgURL;
    export let altImg;
    export let externalURL;
    export let style = 'max-width: 100%; height: auto;';
</script>

<a href={externalURL}>
    <div class="card" style={style}>
        <h1>{title}</h1>
        <p>{description}</p>
        <img src={imgURL} alt={altImg} style={style}>
    </div>
</a>

<style>
    .card {
        border: 1px solid #ccc;
        border-radius: 8px;
        padding: 16px;
        margin: 16px;
    }
</style>
