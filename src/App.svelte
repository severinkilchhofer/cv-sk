<script>
    import Header from './Header.svelte'
    import Paragraph from './Paragraph.svelte'
    import Skill from './Skill.svelte'</script>

<main>
    <div class="container">
        <Header/>

        <div class="row">
            <Paragraph paragraph="Steckbrief"/>
        </div>

        <div class="row">
            <Paragraph paragraph="Erfahrung"/>
        </div>

        <div class="row">
            <Skill skillSection="Programmiersprachen"/>
        </div>

        <div class="row">
            <Skill skillSection="Frameworks und Libraries"/>
        </div>

        <div class="row">
            <Skill skillSection="CI/CD"/>
        </div>

        <div class="row">
            <Skill skillSection="Tools"/>
        </div>

        <div class="row">
            <Paragraph paragraph="Projekte"/>
        </div>

        <div class="row">
            <Paragraph paragraph="Projektunabhängige Aufgaben"/>
        </div>

        <div class="row">
            <Paragraph paragraph="Aus -und Weiterbildung"/>
        </div>

        <div class="row">
            <Paragraph paragraph="Sprachen"/>
        </div>

        <div class="row">
            <Paragraph paragraph="Interessen"/>
        </div>

    </div>
</main>


<style type="text/scss">
    $black: #000000;

    main {
        font-family: 'Montserrat', sans-serif;
        font-weight: 700;
    }


    :global(h1) {
        color: $black;
        font-size: 3em;
        font-weight: 700;
    }

    :global(:root) {


        /* Grid
        –––––––––––––––––––––––––––––––––––––––––––––––––– */
        .container {
            position: relative;
            width: 100%;
            max-width: 960px;
            margin: 0 auto;
            padding: 0 20px;
            box-sizing: border-box;
        }


        .column,
        .columns {
            width: 100%;
            float: left;
            box-sizing: border-box;
        }

        /* For devices larger than 400px */
        @media (min-width: 400px) {
            .container {
                width: 85%;
                padding: 0;
            }
        }

        /* For devices larger than 550px */
        @media (min-width: 550px) {
            .container {
                width: 80%;
            }
            .column,
            .columns {
                margin-left: 4%;
            }
            .column:first-child,
            .columns:first-child {
                margin-left: 0;
            }

            .one.column,
            .one.columns {
                width: 4.66666666667%;
            }
            .two.columns {
                width: 13.3333333333%;
            }
            .three.columns {
                width: 22%;
            }
            .four.columns {
                width: 30.6666666667%;
            }
            .five.columns {
                width: 39.3333333333%;
            }
            .six.columns {
                width: 48%;
            }
            .seven.columns {
                width: 56.6666666667%;
            }
            .eight.columns {
                width: 65.3333333333%;
            }
            .nine.columns {
                width: 74.0%;
            }
            .ten.columns {
                width: 82.6666666667%;
            }
            .eleven.columns {
                width: 91.3333333333%;
            }
            .twelve.columns {
                width: 100%;
                margin-left: 0;
            }

            .one-third.column {
                width: 30.6666666667%;
            }
            .two-thirds.column {
                width: 65.3333333333%;
            }

            .one-half.column {
                width: 48%;
            }


        }


        /* Larger than mobile */
        @media (min-width: 400px) {
        }

        /* Larger than phablet (also point when grid becomes active) */
        @media (min-width: 550px) {
        }

        /* Larger than tablet */
        @media (min-width: 750px) {
        }

        /* Larger than desktop */
        @media (min-width: 1000px) {
        }

        /* Larger than Desktop HD */
        @media (min-width: 1200px) {
        }


    }

</style>