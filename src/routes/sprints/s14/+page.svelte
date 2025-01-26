<section>
    <h1>Lose Your Head // Sprint 14</h1>
    <h2>Inhoudsopgave</h2>
    <ul>
        <li><a href="#repositories">Repositories</a></li>
        <li><a href="#week-1">Week 1</a></li>
        <li><a href="#week-2">Week 2</a></li>
        <li><a href="#week-3">Week 3</a></li>
    </ul>

    <article id="repositories">
        <h3>Repositories</h3>
        <ul>
            <li><a href="link_to_fdnd_we_love_web_repo" target="_blank">FDND We Love Web</a></li>
            <li><a href="link_to_i_love_web_repo" target="_blank">i-love-web</a></li>
        </ul>
    </article>

    <article id="week-1">
        <h3>Week 1 | 23 t/m 27 september</h3>
        <p>In deze sprint zijn we begonnen met Svelte, een component-based framework, en Svelte Kit, een app-framework dat server-side rendering (SSR) ondersteunt.</p>

        <h4>Nieuw project</h4>
        <p>Deze week kregen we een nieuwe opdracht van FDND: het ontwikkelen van een "We Love Web" website. Deze website geeft een overzicht van zowel aankomende als afgelopen We Love Web-sessies, bedoeld voor studenten en docenten. Samen met Jaymar ben ik aan deze opdracht begonnen. We startten met het opzetten van de basis van de site door een sitemap, datamodel en teamcanvas te maken. Dit is allemaal vastgelegd in ons projectboard, dat te vinden is via de volgende link: <a href="link_to_project_board" target="_blank">Project Board FDND We Love Web</a>.</p>
    </article>

    <article id="week-2">
        <h3>Week 2 | 30 september t/m 4 oktober</h3>
        <h4>Mentor dag week 1</h4>
        <p>Tijdens deze week kregen de eerstejaars een college over het grid-systeem. In groepjes werkten ze aan verschillende lay-outs, waarbij ik mijn groepje hielp wanneer ze vastliepen.</p>

        <h4>Structuur en werking overzicht</h4>
        <p>In week 2 werd de structuur en werking van het project verduidelijkt:</p>
        <ul>
            <li><strong>3. Structuur:</strong> De code bevindt zich in de <code>src</code> map. <code>/routes</code> bevat zowel dynamische als statische pagina’s. Server-side code hoort in <code>src/lib/server/</code>.</li>
            <li><strong>2. Routing:</strong> Standaard routing-methodes voor dynamische en statische routes worden toegepast.</li>
            <li><strong>3. Error Handling:</strong> Foutpagina's worden gemaakt via <code>/routes/+error.svelte</code> en <code>/routes/+layout.svelte</code>.</li>
            <li><strong>4. Data Laden:</strong> Data wordt opgehaald met <code>page.js</code> en <code>page.server.js</code>. Server-side functies zijn async.</li>
            <li><strong>5. Binding:</strong> Variabelen worden aan elementen gebonden met <code>bind:value=var</code>.</li>
            <li><strong>6. Library:</strong> Componenten worden geïmporteerd uit <code>src/lib</code> via <code>$lib</code>.</li>
            <li><strong>7. Components:</strong> Je kunt variabelen exporteren binnen componenten met <code>export let variabele</code>.</li>
        </ul>

        <h4>10 Principles of Good Design</h4>
        <p>Hierbij een samenvatting van de 10 principes van goed design:</p>
        <ul>
            <li>Innovatief</li>
            <li>Bruikbaar</li>
            <li>Esthetisch</li>
            <li>Begrijpelijk</li>
            <li>Onopvallend</li>
            <li>Eerlijk</li>
            <li>Duurzaam</li>
            <li>Grondig tot in de details</li>
            <li>Milieuvriendelijk</li>
            <li>Zo minimaal mogelijk</li>
        </ul>

        <h4>Error Page</h4>
        <p>Op basis van Justus' presentatie heb ik een error-pagina gemaakt die gebruik maakt van <code>$page.status</code> om de foutstatus weer te geven.</p>
    </article>

    <article id="week-3">
        <h3>Week 3 | 7 t/m 11 oktober</h3>
        <h4>Waterval vs Agile</h4>
        <p><strong>Waterval:</strong> Hierbij worden alle specificaties van tevoren vastgelegd.</p>
        <p><strong>Agile:</strong> Flexibel en iteratief werken, waarbij aanpassingen mogelijk zijn gedurende het project.</p>

        <h4>FDND Agile Woordenlijst</h4>
        <p>Een lijst van belangrijke termen binnen Agile development:</p>
        <ul>
            <li><strong>Agile Development:</strong> Iteratieve benadering van softwareontwikkeling waarbij teams in korte sprints werken.</li>
            <li><strong>Backlog:</strong> Een prioriteitenlijst met taken die uitgevoerd moeten worden.</li>
            <li><strong>Business Owner:</strong> De persoon die de zakelijke belangen van een project vertegenwoordigt.</li>
            <li><strong>Continuous Integration:</strong> De praktijk waarbij ontwikkelaars regelmatig nieuwe code integreren in de hoofdtak.</li>
            <li><strong>Daily Scrum:</strong> Een dagelijkse bijeenkomst waarin teamleden hun voortgang bespreken.</li>
            <li><strong>Definition of Done:</strong> De criteria waaraan een taak of user story moet voldoen om als voltooid te worden beschouwd.</li>
            <li><strong>Epic:</strong> Een grote user story die kan worden opgedeeld in kleinere, beter beheersbare user stories.</li>
            <li><strong>Feature:</strong> Een functionele eigenschap van een product.</li>
            <li><strong>Iteration:</strong> Een cyclus van een herhalend proces, vaak een korte periode waarin doelen worden bereikt.</li>
            <li><strong>Minimum Viable Product:</strong> De meest eenvoudige versie van een product die nog steeds waarde biedt.</li>
            <li><strong>MoSCoW:</strong> Prioriteringstechniek (Must haves, Should haves, Could haves, Won’t haves).</li>
            <li><strong>Planning Poker:</strong> Een techniek voor het inschatten van de omvang van taken.</li>
        </ul>

        <h4>Layout</h4>
        <p>Met behulp van Justus en Dorien heb ik meer geleerd over het gebruik van layouts in onze projecten. Door gebruik te maken van <code>slot</code>, kan specifieke content geladen worden, terwijl de navigatie en footer consistent blijven op alle pagina's.</p>

        <h4>Mentor Dag Week 2</h4>
        <p>Tijdens deze week heb ik verschillende studenten begeleid:</p>
        <ul>
            <li><strong>Süleyman en Kerem:</strong> Tips gegeven voor het schrijven van een gestructureerde README.</li>
            <li><strong>Mikiyas:</strong> Advies gegeven over wat hij moest afronden voor de sprint review.</li>
            <li><strong>Luuk:</strong> Uitleg gegeven over het maken van een inhoudsopgave in Markdown.</li>
            <li><strong>Arman:</strong> Zijn README nagekeken en geadviseerd om een live link en installatie-instructies toe te voegen.</li>
        </ul>

        <h4>Database</h4>
        <p>Samen met Justus heb ik een database opgezet voor de "We Love Web"-presentaties. Ik heb een datamodel opgesteld dat alle benodigde velden bevat voor een presentatie. Een voorbeeld van een database-item:</p>
        <pre><code>example of database structure</code></pre>

        <h4>Readme</h4>
        <p>Een duidelijke README is van groot belang om toekomstige developers en potentiële sponsoren een goed inzicht te geven in het project. Hier is een voorbeeld van mijn README voor FDND: <a href="link_to_readme" target="_blank">README.md</a></p>

        <h4>Frontend Ontwikkelingen</h4>
        <p>Dit zijn de websites die ik gebruik om up to date te blijven met de laatste ontwikkelingen in de frontend:</p>
        <ul>
            <li><a href="https://dev.to" target="_blank">Dev.to</a></li>
            <li><a href="https://reddit.com/r/webdev" target="_blank">Reddit</a></li>
            <li><a href="https://css-tricks.com" target="_blank">CSS-tricks</a></li>
        </ul>
    </article>
</section>

<style>
    section {
        padding: 4rem 1rem;
        @media (min-width: 1024px) {
            padding: 12rem 0 1rem;
        }
        @media (min-width: 1440px) {
            padding: 7rem 1rem;
        }
        @media (min-width: 1800px) {
            padding: 12rem 1rem;
        }
    }
    section article {
        margin-bottom: 2rem;
        max-width: 30rem;
    }
    h1 {
        margin-bottom: 1.5rem;
    }
    h2 {
        margin-bottom: 1rem;
    }
    h3 {
        margin-bottom: .5rem;
    }
    h4 {
        margin-bottom: .5rem;
    }
    h5 {
        margin-bottom: .5rem;
    }
    p {
        margin: 1rem 0;
    }
    ul {
        color: var(--white);
        font-family: var(--font-text);
    }
    a {
        color: #1e90ff;
        text-decoration: none;
    }
    a:hover {
        text-decoration: underline;
    }
</style>
