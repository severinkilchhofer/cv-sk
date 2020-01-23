<script>
    let mobile = false;

    if (window.screen.width < 500) {
        mobile = true;
    }
</script>

<div class="header-section">
    <div class="row {mobile ? '' : 'alignment'}">
        <div class="{mobile ? 'nine image-center' : 'three'} columns">
            <img src="assets/img/header-image.png" alt="Foto Severin Kilchhofer">
        </div>
        <div class="{mobile ? 'three' : 'nine'} columns">
            <h1>Hallo,<br>
                Ich bin Severin und arbeite als
                Frontend Entwickler und Interaction Designer in Zürich.</h1>
        </div>
    </div>
    <div class="row info-text">
        <div class="three columns offset-by-three">
            <div class="rectangle"></div>
        </div>
    </div>
    <div class="row">
        <div class="nine columns offset-by-three">
            <p>Code und Design zu kombinieren, war immmer mein grösster
                Wunsch. Mit meinem abgeschlossen Studium
                Interaction
                Design kann ich die tägliche Webentwicklung mit UX/UI Design verknüpfen. So ermögliche ich die
                Entwicklung
                erstklassiger Webanwendungen mit konzeptionell durchdachter Navigation und Struktur.</p></div>
    </div>
</div>

<style type="text/scss">
    h1 {
        font-size: 2.6875em;
        margin-block-start: 0;
        margin-block-end: 0;
    }

    p {
        font-weight: 100;
        line-height: 1.5em;
        margin-block-start: -0.4em;
        padding-top: 5em;
    }

    img {
        width: 100%;
    }

    .alignment {
        display: flex;
        align-items: center;
    }

    .image-center {
        text-align: center;
    }

    .info-text {
        padding-top: 3em;
    }

    .header-section {
        height: 80vh;
        padding-top: 25vh;
    }

    .rectangle {
        width: 100%;
        height: 0.6em;
        background-color: #3A64B6;
    }

    @media (max-width: 500px) {
        h1 {
            font-size: 1.3em;
            margin-block-start: 0;
            margin-block-end: 0;
        }

        img {
            width: 60%;
        }
    }

    @media (max-width: 768px) {
        h1 {
            font-size: 1.6em;
        }
    }
</style>
