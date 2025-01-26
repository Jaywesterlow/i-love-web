<section>
    <h1>Your Tribe for Life // Sprint 13</h1>
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
            <li><a href="link_to_profile_card_repo" target="_blank">Profile Card Repository</a></li>
            <li><a href="link_to_squad_page_repo" target="_blank">Squad Page Repository</a></li>
        </ul>
    </article>

    <article id="week-1">
        <h3>Week 1 | 2 t/m 6 september</h3>
        <p>In deze sprint zijn we begonnen met Svelte, een component-based framework, en Svelte Kit, een app-framework dat server-side rendering (SSR) ondersteunt.</p>

        <h4>Leervragen</h4>
        <ul>
            <li>Hoe combineer ik gegevens uit een CMS met een framework?</li>
            <li>Hoe richt ik een project in met een framework?</li>
            <li>Hoe kies ik de juiste tools en frameworks voor een project?</li>
            <li>Wat is de beste manier om mijn learning journal op te zetten?</li>
        </ul>

        <h4>Wat is Svelte en Svelte Kit?</h4>
        <p>Svelte is een JavaScript-framework dat zich onderscheidt door de manier waarop het je code compileert. In plaats van zware runtime libraries, compileert Svelte de code direct naar efficiënte, snelle JavaScript dat meteen in de browser draait. Het is dus lichter en sneller dan veel andere frameworks. Svelte Kit is een uitbreiding van Svelte waarmee je complete web-apps kunt bouwen. Het biedt handige tools voor routing, server-side rendering, API’s en meer, waardoor je in korte tijd een volwaardige app kunt ontwikkelen.</p>

        <h4>Voordelen van Svelte ten opzichte van React</h4>
        <ul>
            <li>Geen runtime overhead: Svelte compileert direct naar JavaScript, dus geen extra runtime nodig.</li>
            <li>Snellere prestaties: Door minder runtime-code presteren Svelte-apps beter en zijn ze kleiner in bestandsgrootte.</li>
            <li>Minder boilerplate: De syntax van Svelte is eenvoudiger en vereist minder code dan React voor dezelfde functionaliteit.</li>
        </ul>

        <h4>Basisinstallatie van Svelte Kit</h4>
        <ol>
            <li>Installeer Node.js.</li>
            <li>Creëer een nieuw project met npm create svelte@latest.</li>
            <li>Kies een projecttemplate.</li>
            <li>Installeer dependencies met npm install.</li>
            <li>Start het project met npm run dev -- --open.</li>
        </ol>

        <h4>Svelte-project opzetten voor de squad page</h4>
        <p>Met behulp van de bovenstaande stappen heb ik een Svelte-project opgezet voor onze squad page. Ik heb de database van Directus gekoppeld via een fetch-json.js bestand in de lib-map, dat de gegevens ophaalt. Vervolgens heb ik een +page.server.js bestand gemaakt voor het renderen van data via een API-link.</p>

        <h4>Bestandstypen in Svelte Kit</h4>
        <ul>
            <li><strong>+page.svelte:</strong> Hier schrijf je HTML, CSS en JavaScript voor een specifieke pagina. Svelte genereert automatisch classes, dus je hoeft je geen zorgen te maken dat stijlen overlappen tussen pagina’s.</li>
            <li><strong>+layout.svelte:</strong> Code die voor alle child routes geldt, zet je hier, zoals een algemene header.</li>
            <li><strong>+page.server.js:</strong> Server-side JavaScript voor de specifieke pagina.</li>
            <li><strong>+layout.server.js:</strong> Server-side code voor alle child routes.</li>
            <li><strong>+server.js:</strong> Hierin kun je API-routes definiëren, zoals GET en POST-methodes.</li>
        </ul>
    </article>

    <article id="week-2">
        <h3>Week 2 | 9 t/m 13 september</h3>
        <h4>Figma workshop</h4>
        <p>In deze workshop kregen we de basis uitgelegd van Figma en enkele handige sneltoetsen om sneller te werken. Voor meer shortcuts kun je deze site checken. Deze week heb ik me beziggehouden met mijn profielkaartje. Ik heb de basis setup geïnstalleerd en een wireframe van de website gemaakt. We hadden afgesproken dat drie teamleden deze week aan hun profielkaart zouden werken en de andere twee aan de squad page. Ik hielp mijn teamgenoten wanneer ze problemen hadden.</p>

        <h4>API-koppeling</h4>
        <p>Voor de API-koppeling maak je een fetch-json.js bestand in de lib-map en gebruik je +page.server.js om de data in te laden. Een voorbeeld van mijn profielkaart is te vinden op deze link.</p>
    </article>

    <article id="week-3">
        <h3>Week 3 | 16 t/m 20 september</h3>
        <h4>MoSCoW & Poker</h4>
        <p>Tijdens de les van maandag hebben we geleerd hoe je de moeilijkheid van een taak kunt inschatten en hoeveel tijd je eraan moet besteden. Ook hebben we het MoSCoW-principe behandeld, waarmee je prioriteiten stelt voor je taken.</p>

        <h4>Van epics naar user stories en taken</h4>
        <p>Epics helpen om werk te organiseren door het op te splitsen in kleinere, overzichtelijke stukken. Dit zorgt ervoor dat projecten beter beheersbaar worden en regelmatig waarde opleveren aan de klant.</p>

        <h5>Epics:</h5>
        <p>Grote projecten zoals het lanceren van een nieuwe website.</p>

        <h5>Stories:</h5>
        <p>Bijvoorbeeld het toevoegen van een winkelmandje.</p>

        <h5>User stories:</h5>
        <p>"Als bezoeker wil ik producten kunnen toevoegen aan mijn winkelmandje om overzicht te houden."</p>

        <h5>Tasks:</h5>
        <p>Concrete taken zoals het ontwerpen van de interface voor het winkelmandje.</p>

        <h4>MoSCoW-methode</h4>
        <ul>
            <li><strong>Must haves:</strong> Deze onderdelen moeten af zijn voor de deadline.</li>
            <li><strong>Should haves:</strong> Belangrijk, maar het project kan doorgaan zonder.</li>
            <li><strong>Could haves:</strong> Leuk om te hebben als er tijd over is.</li>
            <li><strong>Won’t haves:</strong> Goede ideeën, maar geen prioriteit.</li>
        </ul>

        <h4>Hoe lever je een project op?</h4>
        <ul>
            <li><strong>Refactored code:</strong> Geoptimaliseerde en gestructureerde code zonder foutmeldingen.</li>
            <li><strong>README.md:</strong> Beschrijving van het project, installatie-instructies, CMS-handleiding en links.</li>
            <li><strong>Live zetten:</strong> Bijvoorbeeld via GitHub Pages, Vercel, of Netlify.</li>
        </ul>
        <p>Bekijk de live versie van de squad page hier: <a href="link_to_squad_page" target="_blank">Squad Page</a>.</p>
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
