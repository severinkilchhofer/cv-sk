<script>
    import data from './paragraphdata.json'

    export let paragraph;
    const sectionName = data.paragraphs.find(p => p.name === paragraph);
</script>

<section>
    <div class="row">
        <div class="twelve columns">
            <h2>{sectionName.name}</h2>
        </div>
    </div>

    {#each sectionName.attributes as { title, value }}
        <div class="row">
            <div class="three columns">
                <p>{title}</p>
            </div>
            <div class="nine columns">
                <p class="valueText">{value}</p>
            </div>
        </div>
    {/each}
</section>


<style type="text/scss">
    $blue: #3A64B6;

    p {
        margin-block-start: 10px;
        margin-block-end: 10px;
        color: $blue;
    }

    .valueText {
        font-weight: 100;
        color: black;
    }
</style>
