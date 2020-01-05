<script>
    const currentYear = new Date().getFullYear()
</script>

<footer>
    <hr>
    <p>Copyright © {currentYear} Severin Kilchhofer</p>
</footer>

<style>

     footer {
         height: 5vh;
         position: relative;
     }

    p {
        font-size: 0.8em;
        margin: 0;
        top: 50%;
        position: absolute;
        -ms-transform: translateY(-50%);
        transform: translateY(-50%);
    }
</style>