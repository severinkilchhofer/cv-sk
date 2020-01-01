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
                <p class="bold">{title}</p>
            </div>
            <div class="nine columns">
                <p>{value}</p>
            </div>
        </div>
    {/each}
</section>

<style type="text/scss">
    $blue: #3A64B6;

    section {
        margin-top: 2em;
    }

    p {
        margin-block-start: 10px;
        margin-block-end: 10px;
    }

    .bold {
        font-weight: 500;
        color: $blue;
    }

    @media (max-width: 500px) {
        .row:not(:first-child) {
            padding-bottom: 1.3em;
        }
    }
</style>
