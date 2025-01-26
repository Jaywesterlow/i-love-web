<section>
	<h1>Mentoring: 12 Principes van Disney (18-01-2025)</h1>
  
    <article>
        <h2>Sasha</h2>
        <p>
            Ze werkte aan een "return to top"-button. Ik hielp haar met een bug in de document.querySelector, 
            waarbij ze niet de juiste selector had. Hoewel mijn hulp beperkt was, probeerde ik haar zoveel mogelijk 
            te ondersteunen.
        </p>
    </article>

    <article>
        <h2>Miel</h2>
        <p>
            Hij werkte aan een SVG-animatie en een dark mode feature. Ik adviseerde hem om animaties met HTML-elementen 
            te maken in plaats van SVG’s, zodat hij ze makkelijker kon manipuleren met code.
        </p>
    </article>

    <article>
        <h2>Stella</h2>
        <p>
            Ze werkte aan een scale-animation op een button. Ik hielp haar met een probleem waarbij de button horizontaal 
            verschoof vanwege een scale op de parent. Dit gaf haar meer inzicht in de werking van keyframes.
        </p>
    </article>

    <article>
        <h2>Luuk</h2>
        <p>
            Hij werkte aan een CSS popover (popup form met pure CSS), maar ontdekte dat deze niet door Firefox werd ondersteund. 
            Ik legde hem het concept van progressive enhancement (de hadden dit nog niet behandeld) uit en raadde aan om met 
            JavaScript een alternatief voor Firefox te maken.
        </p>
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
        margin-bottom: .5rem;
    }

    p {
        margin: 1rem 0;
    }

    ul {
        color: var(--white);
        font-family: var(--font-text);
    }
</style>
