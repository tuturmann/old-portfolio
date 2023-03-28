<script>
    export let open = false;
    export let handleClick;
</script>

<section>
    <button class:open on:click={handleClick}>
        <div />
        <div />
        <div />
    </button>
</section>

<style>
    button {
        background: none;
        border: none;
    }
    .open > div:first-of-type {
        transform: rotate(45deg) translateY(7px) translateX(7px);
    }
    .open > div:nth-of-type(3) {
        transform: rotate(-45deg) translateY(-7px) translateX(7px);
    }
    .open > div:nth-of-type(2) {
        visibility: hidden;
        opacity: 0;
        transition: visibility 0s 500ms, opacity 500ms linear;
    }

    section div {
        height: 5px;
        width: 25px;
        margin: 5px 0;
        transition-duration: 500ms;
        border-radius: 1px;
    }
    section div:first-of-type {
        background-color: #e2714b;
    }

    section div:nth-of-type(2) {
        background-color: #e2714b;
        visibility: visible;
        opacity: 1;
        transition: opacity 500ms linear;
    }

    section div:nth-of-type(3) {
        background-color: #e2714b;
    }
</style>
