<script>
    import skilldata from './skilldata.json'

    export let skillSection;
    const data = skilldata.skillsection.find(s => s.name === skillSection);
</script>

<section>
    <div class="row">
        <div class="twelve columns">
            <h2>{data.name}</h2>
        </div>
    </div>

    <div class="row">
        {#each data.attributes as { skill, active }}
            <div class="three columns">
                <div class="skill-card" class:active="{active === true}">
                    <p>{skill}</p>
                </div>
            </div>
        {/each}
    </div>
</section>


<style type="text/scss">
    $blue: #3A64B6;
    $black: #000000;

    section {
        margin-top: 2em;
    }

    .skill-card {
        width: 100%;
        height: 4.1875em;
        border-radius: 4px;
        background-color: $black;
        color: white;
        font-weight: 600;
        text-align: center;
        vertical-align: middle;
        line-height: 4.1875em;
    }

    .three:nth-child(5),
    .three:nth-child(9) {
        margin-left: 0;
    }

    .active {
        background-color: $blue;
    }

</style>
