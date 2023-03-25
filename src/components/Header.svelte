<script>
    import Fa from "svelte-fa";
    import { faStar, faBars } from "@fortawesome/free-solid-svg-icons";
    import {
        faGithub,
        faArtstation,
        faLinkedin,
    } from "@fortawesome/free-brands-svg-icons";
</script>

<head>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link
        rel="preconnect"
        href="https://fonts.gstatic.com"
        crossorigin="anonymous"
    />
    <link
        href="https://fonts.googleapis.com/css2?family=Cormorant+Upright:wght@600&display=swap"
        rel="stylesheet"
    />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link
        rel="preconnect"
        href="https://fonts.gstatic.com"
        crossorigin="anonymous"
    />
    <link
        href="https://fonts.googleapis.com/css2?family=Electrolize&display=swap"
        rel="stylesheet"
    />
</head>

<header>
    <div>
        <span class="icon">
            <Fa icon={faStar} />
        </span>
        <span class="Manon"> Manon </span>
        <a
            class="icon"
            href="https://www.linkedin.com/in/manon-leclercq-789108264/"
        >
            <Fa icon={faLinkedin} />
        </a>
        <a class="icon" href="https://github.com/tuturmann">
            <Fa icon={faGithub} />
        </a>
        <a class="iconArt" href="https://www.artstation.com/manonlclq5">
            <Fa icon={faArtstation} />
        </a>
    </div>

    <nav>
        <a href="/"> à propos </a>
        <a href="/informatique"> informatique </a>
        <a href="/artiste"> artiste </a>
        <Fa icon={faBars} />
    </nav>
</header>

<style>
    nav > a {
        margin: 0 20px;
        font-size: 20px;
        color: #e1e6e1;
    }

    div > a {
        margin: 0 5px;
    }

    header {
        display: flex;
        justify-content: space-between;
        font-size: 30px;
        padding: 10px;
    }

    .icon {
        color: #e2714b;
    }

    .iconArt {
        color: #996888;
    }

    span {
        color: #e1e6e1;
    }

    .Manon {
        font-family: "Cormorant Upright", serif;
    }

    nav {
        color: #e1e6e1;
        font-family: "Electrolize", sans-serif;
    }

    nav > a:visited {
        color: #e1e6e1;
    }

    nav > a:link {
        text-decoration: none;
    }
    nav > a:hover {
        text-decoration: underline;
        transition: 2s;
    }
</style>
