<script>
    import { Navigation } from "$lib";

</script>

<Navigation />

<main>
    <article>
        <h1>Hey, This is currently still under construction! 🚧</h1>
        <p>but you can view the I Love Web page <a href="i-love-web">here!</a></p>
    </article>
</main>

<style>
    main {
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
        }
    }

    main article h1 {
        margin-bottom: 1rem;
    }

    main article p a {
        text-decoration: none;
        color: cornflowerblue;
    }
</style>
