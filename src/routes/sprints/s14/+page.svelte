<script>
    import { Navigation, Svg } from "$lib";

</script>

<Navigation />

<main>
    <a href="../i-love-web"><Svg name="return"/></a>
    <article>
        <h1>Sprint 13</h1>
        <p>this is the sprint 13 documentation!</p>
    </article>
</main>

<style>
    main {
        padding: 0 5%;
        position: relative;
        height: 70%;
        width: 100%;
        display: flex;
        flex-direction: column;
        text-align: center;
        justify-content: center;
        align-items: center;
        font-family: var(--font-title);
        color: var(--white);
        font-size: .8rem;

        @media (min-width: 1024px) {
            font-size: 1.5rem;
            padding: 0 10%;
        }
    }

    main > a {
        position: absolute;
        left: 5%;
        top: 0;

        @media (min-width: 1024px) {
            left: 10%;
        }
    }

    main article h1 {
        margin-bottom: 1rem;
    }
</style>