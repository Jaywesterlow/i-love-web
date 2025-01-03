<script>
    import { Navigation, Hero } from "$lib";

</script>

<Navigation />

<main>
    <Hero />
</main>



<style>
    main {
        width: 100%;
        background: var(--bg);
        border-radius: 1.563rem;
        padding: 3.125rem 5%;
    }

    @media screen and (min-width: 768px) {
        main {
            border-radius: 1.875rem;
            padding: 1rem 3.125rem 1rem;
        }
    }

    @media screen and (min-width: 1024px) {
        main {
            border-radius: 2.5rem;
            padding: 1rem 10%;
        }
    }
</style>