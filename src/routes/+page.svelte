<script>
    import Header from "../components/Header.svelte";
</script>

<svelte:head>
    <title>A propos</title>
    <meta name="description" content="Portfolio Manon Leclercq" />
</svelte:head>

<section>
    <Header />
    <main>
        <div>
            <span class="mainManon"> Leclercq Manon </span>

            <img class="main-image" alt="main" src="/assets/main-image.jpg" />
        </div>

        <div>
            <h1>Bienvenue</h1>

            <p>
                Etudiante en BUT Informatique, je recherche une alternance en
                informatique pour ma deuxième et troisième année de BUT.
            </p>

            <h1>Contact</h1>

            <p>
                mmanon.leclercq@gmail.com <br />
                Mon compte
                <a href="https://www.linkedin.com/in/manon-leclercq-789108264/">
                    LinkedIn
                </a>
            </p>
        </div>
    </main>

    <div class="footerUnPeu">
        <p>passionnée aussi par les</p>
        <span class="paragraphBig"> Langues étrangères </span>
        <p>
            • Bilingue français/anglais <br />
            • Niveau A2 en espagnol<br />
            • J’ai commencé à apprendre le turc, le russe et le japonais.<br />
        </p>
    </div>
</section>

<style>
    a:link {
        color: #e3d26f;
        text-decoration: none;
    }

    a:hover {
        text-decoration: underline;
    }

    a:visited {
        color: #e3d26f;
    }

    main > div:first-of-type {
        position: relative;
    }
    section {
        margin: 0px;
        background-color: #243529;
        border: 10px solid #b0a990;
        box-sizing: border-box;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        min-height: 100vh;
    }
    main {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
    }
    .main-image {
        border-radius: 25px;
        width: 315px;
        object-fit: cover;
        position: relative;
        z-index: 10;
        filter: brightness(0.5);
    }

    .mainManon {
        color: #e1e6e1;
        font-family: "Electrolize", sans-serif;
        font-size: 50px;
        position: absolute;
        z-index: 11;
        border: 5px double #243529;
        margin: 20px;
    }

    h1 {
        color: #e2714b;
        font-family: "Electrolize", sans-serif;
        font-size: 40px;
        font-weight: 400;
        margin: 5px;
        text-align: center;
    }

    p {
        color: #e1e6e1;
        font-family: "Electrolize", sans-serif;
        font-size: 25px;
        text-align: center;
        max-width: 300px;
    }

    .paragraphBig {
        color: #e1e6e1;
        font-family: "Electrolize", sans-serif;
        font-size: 40px;
    }

    .footerUnPeu {
        background: rgba(
            108,
            57,
            57,
            0.33
        );
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        margin: 0px;
    }
</style>
