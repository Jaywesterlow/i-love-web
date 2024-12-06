<script>
    import { Navigation } from "$lib";

    let showList = false;

    function toggleVisibility() { 
        showList = !showList;
    }

    
</script>

<Navigation />

<main>
  <article class:fade-out={showList}>
    <h1>Welcome to the I love web page!</h1>
    <p>Here you can view my <button on:click={toggleVisibility}>documentation.</button></p>
  </article>
  
  <ul class:fade-in={showList}>
    <li><a href="sprints/s13">Sprint 13: Tribe For Life</a></li>
    <li><a href="sprints/s14">Sprint 14: Lose Your Head</a></li>
    <li><a href="sprints/s15">Sprint 15: Choices, Choices</a></li>
    <li><a href="sprints/s16">Sprint 16: Don't Repeat Yourself</a></li>
    <li><a href="sprints/s17">Sprint 17: User Needs</a></li>
  </ul>
</main>


<style>
    main {
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
        }
    }

    main article {
        transition: opacity 300ms;
        pointer-events: auto; /* Ensure interaction when visible */
    }

    main article.fade-out {
        opacity: 0;
        pointer-events: none; /* Prevent interaction when hidden */
    }

    main ul {
        transition: opacity 300ms;
        opacity: 0;
        pointer-events: none; /* Prevent interaction when hidden */
    }

    main ul.fade-in {
        opacity: 1;
        pointer-events: auto; /* Ensure interaction when visible */
    }


    
    main article h1 {
        margin-bottom: 1rem;
    }

    main article p {
        display: flex;
        justify-content: center;

    }

    main article p button {
        color: cornflowerblue;
        font-family: var(--font-title);
        font-size: .8rem;
        background-color: transparent;
        background-repeat: no-repeat;
        border: none;
        cursor: pointer;
        overflow: hidden;
        outline: none;
        display: block;
        position: relative;
        transition: 300ms;
        padding: 0 0 .2rem .5rem;


        @media (min-width: 1024px) {
            font-size: 1.5rem;
        }
    }

    main article p button::after {
        content: "" ;
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 0.1em;
        background-color: cornflowerblue;
        transition: opacity 300ms, transform 300ms;
        transform: translate3d(-101%, 0, 0);
        opacity: 1;
        }

        main article p button:hover::after,
        main article p button:focus::after{
            transform: translate3d(0, 0, 0);
        }

        main ul {
            position: absolute;
            list-style-type: none;
            text-align: left;
        }

        main ul li:not(:last-child) {
            padding-bottom: 1rem;
        }
</style>
