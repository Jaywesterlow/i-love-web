<script>
	import { Navigation, Svg } from '$lib';
</script>

<Navigation />

<main>
	<a href="../i-love-web"><Svg name="return" /></a>

	<section>
		<header>
			<h1>User Needs</h1>
			<small>Sprint 16</small>
		</header>

		<h2>Inhoudsopgave</h2>
		<ul>
			<li><strong>Repositories</strong></li>
			<li>
				<strong>Week 1</strong>
				<ul>
					<li>Component Library</li>
					<li>RAP/PE-Websites</li>
					<li>Quality Assurance</li>
					<li>Don’t Repeat Yourself</li>
					<li>Morfologische Kaart</li>
					<li>CSS Weekly</li>
					<li>Typografie en Fonts</li>
				</ul>
			</li>
			<li>
				<strong>Week 2</strong>
				<ul>
					<li>Mentor dag week 4</li>
					<li>Component Library 2</li>
					<li>Functional layering</li>
					<li>Svelte 5</li>
					<li>Responsive to the user</li>
				</ul>
			</li>
		</ul>

		<article>
			<h2>Repositories</h2>
			<ul>
				<li>
					<a href="https://github.com/fdnd-task/dont-repeat-yourself-component-library"
						>Component Library</a
					>
				</li>
				<li><a href="https://github.com/Remy2072/i-love-web">i-love-web</a></li>
			</ul>
		</article>

		<article>
			<h2>Week 1 | 11 t/m 15 november</h2>
			<p>
				Tijdens deze eerste week ligt de focus op het opzetten van een solide basis voor het project
				door structuur en consistentie aan te brengen in de code en ontwerpbenadering. Hierbij
				worden de volgende stappen genomen:
			</p>

			<h3>Component Library</h3>
			<p>
				Een component library is een verzameling van vooraf gemaakte, geteste, en goed
				gedocumenteerde UI-componenten die herbruikbaar zijn. Dit bevordert consistentie,
				efficiëntie, en schaalbaarheid.
			</p>

			<h3>RAP/PE-Websites</h3>
			<p>De websites moeten voldoen aan de volgende richtlijnen:</p>
			<ul>
				<li><strong>Responsive:</strong> Geschikt voor verschillende schermformaten.</li>
				<li><strong>Accessible:</strong> Toegankelijk voor alle gebruikers.</li>
				<li><strong>Performance:</strong> Optimale prestaties en korte laadtijden.</li>
				<li>
					<strong>Progressive Enhancement:</strong> Basisfunctionaliteit gegarandeerd, verbeteringen
					voor moderne browsers.
				</li>
			</ul>

			<h3>Quality Assurance</h3>
			<p>
				Door deze aanpak wordt de kwaliteit van de UI-componenten gewaarborgd, wat leidt tot een
				duurzame en stabiele gebruikerservaring.
			</p>

			<h3>Don’t Repeat Yourself (DRY)</h3>
			<p>
				Vermijd dubbele of overbodige code om de leesbaarheid en onderhoudbaarheid van het project
				te verbeteren.
			</p>

			<h3>Morfologische Kaart</h3>
			<p>
				Een morfologische kaart is een ontwerp tool waarmee je systematisch verschillende
				oplossingen voor een complex probleem kunt verkennen:
			</p>
			<ul>
				<li>
					<strong>Definieer functies:</strong> Bepaal de belangrijkste aspecten van het ontwerp.
				</li>
				<li>
					<strong>Bedenk varianten:</strong> Maak een lijst met mogelijke oplossingen voor elke functie.
				</li>
				<li><strong>Vul de matrix:</strong> Organiseer functies en varianten in een tabel.</li>
				<li>
					<strong>Combineer en evalueer:</strong> Creëer opties en beoordeel ze op criteria zoals kosten
					en haalbaarheid.
				</li>
			</ul>

			<h3>CSS Weekly</h3>
			<p>
				Justus raadde ons aan om ons te abonneren op CSS Weekly, een gerenommeerde nieuwsbrief voor
				waardevolle inzichten in CSS-ontwikkelingen.
			</p>

			<h3>Typografie en Fonts</h3>
			<p>
				Vergelijk de fonts die je wilt gebruiken met de woorden op je website en experimenteer met
				verschillende combinaties. Typografie is 95% van webdesign.
			</p>

			<h3>Variable Fonts</h3>
			<ul>
				<li>
					Eén bestand voor meerdere stijlen zoals breedte en gewicht: <a
						href="https://variablefonts.io">variablefonts.io</a
					>
				</li>
				<li>
					Check je fontvariaties op: <a href="https://wakamaifondue.com">wakamaifondue.com</a>
				</li>
			</ul>
		</article>

		<article>
			<h2>Week 2 | 18 t/m 22 november</h2>

			<h3>Component Library 2</h3>
			<p>
				Een verzameling herbruikbare en generieke componenten die het project consistent en
				onderhoudbaar maken.
			</p>

			<h3>Functional Layering</h3>
			<ul>
				<li><strong>Inputs:</strong> Knoppen, kaartjes.</li>
				<li><strong>Display:</strong> Tabellen, grafieken.</li>
				<li><strong>Navigatie:</strong> Headings, footers, menu’s.</li>
				<li><strong>Structuur:</strong> Grids, containers.</li>
			</ul>

			<h3>Svelte 5</h3>
			<p><strong>New features:</strong> Runes, $props, en Snippets.</p>

			<h3>Responsive Design</h3>
			<p>
				Rekening houden met gebruikersvoorkeuren, container queries, en vouwbare schermen via @media
				(spanning).
			</p>
		</article>
	</section>
</main>

<style>
	* {
		font-size: 1.125rem;
		line-height: 1.5;
	}

	main {
		padding: 0 5%;
		position: relative;
		width: 100%;
		color: var(--white);

		@media (min-width: 1024px) {
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

	section {
		display: flex;
		align-items: left;
		flex-direction: column;
		justify-content: center;
		padding: 0 10% 2rem 10%;
	}

	header {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	header h1 {
		font-size: 2.2rem;
    font-family: var(--font-title);
	}

	small {
		margin-top: .75rem;
		font-size: 1.25rem;
		font-weight: 300;
	}

	h2 {
		margin-top: 1.875rem;
		font-size: 1.563rem;
    font-family: var(--font-title);
	}

	h3 {
		margin-top: 1.25rem;
		font-size: 1.125rem;
		color: rgb(253, 253, 231);
    font-family: var(--font-title);
	}

  p {
    font-family: var(--font-text);
  }

	ul {
		list-style-type: revert;
		padding-left: 1.25rem;
    font-family: var(--font-text);
	}
	ul li {
		margin-bottom: 0.5em;
	}
	ul li ul {
		margin-left: 1.25rem;
	}

	a {
		color: rgb(0, 255, 213);
		text-decoration: underline;
		margin: 0;
    font-family: var(--font-alt);

	}

	@media (min-width: 600px) {
		section {
			padding: 0 20%;
		}
	}

	@media (min-width: 900px) {
		section {
			padding: 0 30%;
		}

		h1 {
			font-size: 3.125rem;
		}

		h2 {
			font-size: 1.563rem;
		}
	}

	@media (min-width: 1300px) {
		section {
			padding: 0 35%;
		}
	}
</style>
