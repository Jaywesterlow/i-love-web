<script>
    import { Navigation } from "$lib";
</script>

<Navigation />

<main>
    <slot/>
</main>

<style>
    main {
        
        margin-top: 87px;
        @media (min-width: 1024px) {
            margin-top: 119px;
        }
    }
</style>
