<script>
    import Header from './Header.svelte'
    import Paragraph from './Paragraph.svelte'
    import Skill from './Skill.svelte'
    import Footer from './Footer.svelte'
    import Legend from './Legend.svelte'</script>

<main>
    <div class="container">
        <Header/>
        <Paragraph paragraph="Steckbrief"/>
        <Paragraph paragraph="Erfahrung"/>
        <Skill skillSection="Programmiersprachen"/>
        <Skill skillSection="Frameworks und Libraries"/>
        <Skill skillSection="CI/CD"/>
        <Skill skillSection="Tools"/>
        <Legend/>
        <Paragraph paragraph="Projekte"/>
        <Paragraph paragraph="Projektunabhängige Aufgaben"/>
        <Paragraph paragraph="Aus- und Weiterbildung"/>
        <Paragraph paragraph="Sprachen"/>
        <Paragraph paragraph="Interessen"/>
        <Footer/>
    </div>
</main>


<style type="text/scss">
    $black: #000000;

    /* Fonts
–––––––––––––––––––––––––––––––––––––––––––––––––– */

    @font-face {
        font-family: Circ-Black;
        src: url(/assets/fonts/CircularStd-Black.woff2) format('woff2'),
        url(/assets/fonts/CircularStd-Black.woff) format('woff'),
        url(/assets/fonts/CircularStd-Black.ttf) format('ttf')
    }

    @font-face {
        font-family: Circ-Bold;
        src: url(/assets/fonts/CircularStd-Bold.woff2) format('woff2'),
        url(/assets/fonts/CircularStd-Bold.woff) format('woff'),
        url(/assets/fonts/CircularStd-Bold.ttf) format('ttf')
    }


    @font-face {
        font-family: Circ-Book;
        src: url(/assets/fonts/CircularStd-Book.woff2) format('woff2'),
        url(/assets/fonts/CircularStd-Book.woff) format('woff'),
        url(/assets/fonts/CircularStd-Book.ttf) format('ttf')
    }

    @font-face {
        font-family: Circ-Medium;
        src: url(/assets/fonts/CircularStd-Medium.woff2) format('woff2'),
        url(/assets/fonts/CircularStd-Medium.woff) format('woff'),
        url(/assets/fonts/CircularStd-Medium.ttf) format('ttf')
    }

    main {
        font-family: 'Circ-Book', sans-serif;
    }


    :global(h1) {
        color: $black;
        font-size: 3em;
        font-family: 'Circ-Black', sans-serif;
    }

    :global(h2) {
        font-family: 'Circ-Bold', sans-serif;
    }

    @media (max-width: 500px) {
        :global(h1) {
            font-size: 1.4em;
        }
        :global(h2) {
            font-size: 1.2em;
        }
    }


    /* Grid
–––––––––––––––––––––––––––––––––––––––––––––––––– */

    :global(:root) {
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

        /* Self Clearing Goodness */
        .container:after,
        .row:after,
        .u-cf {
            content: "";
            display: table;
            clear: both;
        }


    }

</style>