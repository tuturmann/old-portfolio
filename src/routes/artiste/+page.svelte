<script>
    import Header from "../../components/Header.svelte";
</script>

<section>
    <!-- faire la barre marron en haut, mettre les svg, positionner les trucs -->

    <span class="title">
        <a href="https://manonlclq5.artstation.com">
            &gt; Mon portfolio d'artiste &lt;
        </a>
    </span>

    <!-- LOGICIELS -->
    <div>
        <div>
            <span class="title"> Logiciels </span>

            <span class="paragraph">
                Passionnée par le dessin depuis mes 9 ans, je maîtrise les
                logiciels de dessin tels que <span class="software">Clip Studio Paint</span> et <span class="software">PaintTool SAI</span>.
            </span>
        </div>

        <img alt="blender" src="assets/svg_painting.svg" />
    </div>
    <!-- PROJETS -->
    <div>
        <div>
            <span class="title"> Projets professionnels et personnels </span>

            <span class="paragraph">
                J’ai réalisé des assets pour les jeux que je réalise à l’IUT
                mais aussi des dessins juste en tant qu’hobby.
            </span>
        </div>
        <img alt="love" src="assets/svg_love.svg" />
    </div>

    <!-- BLENDER -->
    <div>
        <div>
            <span class="title"> Blender </span>

            <span class="paragraph">
                J’ai récemment commencé à prendre en main <span class="software">Blender</span>. J'ai réalisé
                quelques modèles 3D.
            </span>
        </div>
        <img alt="blender" src="assets/svg_blender.svg" />
    </div>
</section>

<style>

    .software {
        color: #e2714b;
    }
    .title {
        font-family: "Electrolize", sans-serif;
        font-size: 32px;
        color: #e1e6e1;
    }

    .paragraph {
        font-family: "Electrolize", sans-serif;
        font-size: 19px;
        color: #e1e6e1;
    }

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
</style>
