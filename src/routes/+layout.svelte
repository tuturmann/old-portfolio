<script>
    import Fa from "svelte-fa";
    import { faStar } from "@fortawesome/free-solid-svg-icons";
    import {
        faGithub,
        faArtstation,
        faLinkedin,
    } from "@fortawesome/free-brands-svg-icons";
    import Cheeseburger from "../components/Cheeseburger.svelte";
    let open = false;
    function handleClick() {
        open = !open;
    }


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
        <div class:open>
            <a href="/"> à propos </a>
            <a href="/informatique"> informatique </a>
            <a href="/artiste"> artiste </a>
        </div>
            
        <Cheeseburger {open} {handleClick} />
    </nav>
</header>
<section>   
    <slot/>
</section>

<style>
    .open {
        visibility: visible;
        transform: translate(0,-3px);
    }

    nav>div{
        transform: translate(0, -200px);
        visibility:hidden;
        transition: 500ms;
    }
    nav {
        margin: 0 10px;
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
        background: url(/assets/bg-grain-dark.png), #3c372e;
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
        display: flex;
        justify-content: center;
        align-items: center;
    }

    nav a:visited {
        color: #e1e6e1;
    }

    nav a:link {
        color: #e1e6e1;
        text-decoration: none;
    }
    nav a:hover {
        text-decoration: underline;
    }
    section{
        margin: 0px;
        background: url(/assets/bg-grain-dark.png), #243529;
        border: 2px solid #b0a990;
        box-sizing: border-box;
        display: flex;
        height: 100%;
        flex-direction: column;
    }    
</style>
