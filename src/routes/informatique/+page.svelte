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

    <span class="title">
        Les aspects de l'informatique qui m'intéressent :
    </span>
    <!-- DEVELOPPEMENT D'APPLICATIONS -->
    <div>
        <div>
            <span class="title"> Développement </span>

            <span class="paragraph">
                J'aime réaliser des <span class="language">jeux vidéo</span>, concevoir des univers, développer des personnages et construire des défis pour les joueurs. <br>
                En tant que créatrice de jeux vidéo, j'aimerais pouvoir combiner mes compétences en programmation avec mon intérêt artistique. <br>
                <br>
                De plus, le développement de <span class="language">logiciels d'entreprise</span> m'intéresse. J’aime réaliser des applications qui résolvent des problèmes et satisfont l'utilisateur. <br> 
                <br> Ces deux possibilités de développement me permettraient d'être stimulée intellectuellement, car ce sont des domaines en évolution constante. <br>
                <br> Connaissances en <span class="language">Java</span>.
            </span>
        </div>

        <img alt="software development" src="assets/svg_software.svg" />
    </div>
    <!-- ADMINISTRATION SYSTEME -->
    <div>
        <div>
            <span class="title"> Administration système </span>

            <span class="paragraph">
                J’aime automatiser mes tâches et paramétrer un système. Pour moi, Linux représente un véritable terrain de jeu pour l'exploration et la personnalisation.
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
                J'aimerais faire partie de ceux qui travaillent pour améliorer la sécurité du monde informatique. Je suis motivée pour participer à créer des solutions qui permettront de limiter les menaces en ligne.
                <br> Le métier de PenTester m'intéresse en particulier dans le domaine de la cybersécurité.
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
                web. Mes connaissances en <span class="language"> Svelte </span> sont encore en développement, mais je suis impatiente de développer davantage mes compétences.
            </span>
        </div>

        <img alt="web" src="assets/svg_web.svg" />
    </div>
</section>

<style>
    img {
        width: 400px;
        margin: 100px;
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
        text-align: center;
    }

    .language {
        color: #e2714b;
    }
    
    section > div:nth-child(even) {
        margin: 200px 0;
        display: flex;
        justify-content: space-around;
        flex-direction: row-reverse;
    }

    section > div:nth-child(odd) {
        margin: 200px 0;
        display: flex;
        justify-content: center;
    }

</style>
