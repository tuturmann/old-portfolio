<script>
    import { now } from "svelte/internal";
    import Header from "../components/Header.svelte";

    function calculateMyAge() {
        const today = new Date();
        const birthDay = new Date(2004, 11, 5); // month is 0-11, 5th Dec 2004
        let age = today.getFullYear() - birthDay.getFullYear();
        const m = today.getMonth() - birthDay.getMonth();
        if (m < 0 || (m === 0 && today.getDate() < birthDay.getDate())) {
            age--;
        }
        return age;
    }
</script>

<svelte:head>
    <title>A propos</title>
    <meta name="description" content="Portfolio Manon Leclercq" />
</svelte:head>

<section>
    <main>
        <div>
            <span class="mainManon"> Leclercq Manon </span>

            <img class="main-image" alt="main" src="/assets/main.jpg" />
        </div>

        <div>
            <h1>Bienvenue</h1>

            <p>
                J'ai { calculateMyAge() } ans et je suis étudiante en deuxième année de BUT Informatique, je recherche un <em>stage</em> en 
                développement d'applications/web du 15 avril à fin juin 2024. (10 semaines)
            </p>

            <h1>Contact</h1>

            <p class="contacts">
                <a href="/CV.pdf" target='_blank'>Mon CV</a><br/>
                <a href="mailto:mmanon.leclercq@gmail.com">
                    mmanon.leclercq@gmail.com
                </a> <br />
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
            • Débutante en turc (en autodidacte).<br />
        </p>
    </div>
</section>

<style>
    .contacts a {
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
    
    main {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        margin: 40px;
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
        font-size: 70px;
        position: absolute;
        z-index: 11;
        margin: 0 -50px;
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
        background: rgba(108, 57, 57, 0.33);
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        margin: 10px;
    }

    @media screen and (max-width:750px){
        main{
            flex-direction: column;

        }

        .main-image{
            width: 90%;
        }

        div>p>a:first-of-type{
            word-wrap: break-word;
        }

        .paragraphBig{
            text-align: center;
        }

        .mainManon{
            font-size: 2em;
            margin-left: auto;
        }
    }
</style>
