<script>
	import { SortButton } from '$lib';
</script>

<section>
	<h2>I Love Web</h2>

	<picture>
		<img src="" alt="" />
		<article>
			<h3>I Love Web</h3>
			<p></p>
			<ul>
				<li><SortButton /></li>
				<li><SortButton /></li>
				<li><SortButton /></li>
			</ul>
		</article>
	</picture>

	<article>
		<ul>
			<h3>Sprints</h3>
      <li><a href="/sprints/s13">Sprint 13 docs</a></li>
      <li><a href="/sprints/s14">Sprint 14 docs</a></li>
      <li><a href="/sprints/s15">Sprint 15 docs</a></li>
      <li><a href="/sprints/s16">Sprint 16 docs</a></li>
      <li><a href="/sprints/s17">Sprint 17 docs</a></li>
      <li><a href="/sprints/s18">Sprint 18 docs</a></li>
		</ul>

		<ul>
			<h3>We Love Webs</h3>
      <li><a href="/wlw/s13">S13 - Vasilis van Gemert</a></li>
      <li><a href="/wlw/s14">S14 - Nicolas Garnier</a></li>
      <li><a href="/wlw/s15">S15 - Dion Pieters</a></li>
      <li><a href="/wlw/s16">S16 - Emiel van Betsbrugge</a></li>
      <li><a href="/wlw/s17">S17 - Justus Sturkenboom</a></li>
      <li><a href="/wlw/s18">S18 - Dave Bitter</a></li>
		</ul>

		<ul>
			<h3>Mentoring</h3>
      <li><a href="/mentor/s3">Sprint 3 docs</a></li>
      <li><a href="/mentor/s5">Sprint 5 docs</a></li>
      <li><a href="/mentor/s6">Sprint 6 docs</a></li>
		</ul>
	</article>
</section>

<style>
	section {
		min-height: 80vh;
		margin-top: 87px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    padding: 4rem 0;
		@media (min-width: 1024px) {
			margin-top: 119px;
		}
	}

  section h2 {
    position: absolute;
    top: 0rem;
    left: 0;
  }

	picture {
		display: none;
	}

  section article {
    display: flex;
    flex-direction: column;
    gap: 4rem;
    @media (min-width: 1024px) {
			flex-direction: row;
		}
  }

  section article ul {
    list-style-type: none;
    font-family: var(--font-text);
  }

  section article ul h3 {
    margin-bottom: 1rem;
  }
  
  section article ul li {
    margin-bottom: .5rem;
  }
  
  section article ul li a {
    text-decoration: underline;
    color: var(--white);

  }

</style>
