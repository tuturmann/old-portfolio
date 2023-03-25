<script>
    import Header from "../../components/Header.svelte";
</script>

<svelte:head>
    <title>Informatique</title>
    <meta
        name="description"
        content="Portfolio Manon Leclercq : section Informatique"
    />
</svelte:head>

<section>
    <!-- faire la barre marron en haut, mettre les svg, positionner les trucs -->

    <Header />

    <span class="title">
        Les aspects de l'informatique qui m'intéressent :
    </span>
    <!-- DEVELOPPEMENT D'APPLICATIONS -->
    <div>
        <div>
            <span class="title"> Développement d'applications </span>

            <span class="paragraph">
                J’aime réaliser des applications qui satisfont l’utilisateur.
                Connaissances en <span class="language">Java</span>.
            </span>
        </div>

        <img alt="software development" src="assets/svg_software.svg" />
    </div>
    <!-- ADMINISTRATION SYSTEME -->
    <div>
        <div>
            <span class="title"> Administration système </span>

            <span class="paragraph">
                J’aime automatiser mes tâches et paramétrer un système.
                Connaissances en <span class="language">Bash</span> et
                <span class="language">Python</span>.
            </span>
        </div>

        <img alt="system" src="assets/svg_system.svg" />
    </div>
    0
    <!-- CYBERSECURITE -->
    <div>
        <div>
            <span class="title"> Cybersécurité </span>

            <span class="paragraph">
                Je veux participer à rendre le monde informatique plus sûr.
            </span>
        </div>

        <img alt="cybersecurity" src="assets/svg_cybersecurity.svg" />
    </div>
    <!-- DEVELOPPEMENT WEB -->
    <div>
        <div>
            <span class="title"> Développement Web </span>

            <span class="paragraph">
                J'aime exprimer ma créativité au travers de la création de sites
                web. Connaissances en <span class="language">Svelte</span>.
            </span>
        </div>

        <img alt="web" src="assets/svg_web.svg" />
    </div>
</section>

<style>
    section {
        margin: 0px;
        background-color: #243529;
        border: 10px solid #b0a990;
        box-sizing: border-box;
        display: flex;
        height: 100%;
        flex-direction: column;
    }

    img {
        width: 400px;
    }

    div > div {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        margin: 0px 150px;
    }

    .title {
        font-family: "Electrolize", sans-serif;
        font-size: 32px;
        color: #e1e6e1;
        display: flex;
        justify-content: center;
        margin-top: 50px;
    }

    .paragraph {
        font-family: "Electrolize", sans-serif;
        font-size: 19px;
        color: #e1e6e1;
    }

    .language {
        color: #e2714b;
    }

    section > div:nth-child(even) {
        margin: 200px 0;
        display: flex;
        justify-content: center;
        flex-direction: row-reverse;
    }

    section > div:nth-child(odd) {
        margin: 200px 0;
        display: flex;
        justify-content: center;
    }
</style>
