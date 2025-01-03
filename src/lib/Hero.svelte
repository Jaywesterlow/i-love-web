<script>
	import { Svg } from '$lib';
</script>

<section>
	<h1>Jaymar Westerlow, Web designer- & Developer</h1>

  <ul>
    <li><Svg name="portrait" /></li>
    <li><Svg name="logo" /></li>
    <li>WEB DESIGNER</li>
    <li>& DEVELOPER</li>
  </ul>

  <div>
    <ul>
      <li>CONNECT WITH ME:</li>
      <li>Insta</li>
      <li>Link</li>
    </ul>

    <article>
      <p>
        Hello, I’m <span>Jaymar</span> -I design and develop  <span>web-apps</span> and specialize in <span>accessibility</span> and <span>performance</span>. I focus on creating unique, memorable designs while maintaining <span>clean</span>, <span>professional</span> standards.
      </p>
    </article>
    <aside>
      <button>CONTACT ME</button>
    </aside>
  </div>
</section>

<style>
  section {
  }
  
  section h1 {
    display: none;
  }

  section > ul {
    font-family: var(--font-title);
    font-weight: var(--font-bold);
    color: var(--white);
    display: flex;
    flex-direction: column;
    align-items: center;
    font-size: 2rem;
    list-style-type: none;

    @media (min-width: 500px) {
      font-size: 2.5rem;
    }
  }

  section > ul > li:nth-child(1) {
    margin-bottom: 3rem;
  }

  section > ul > li:nth-child(2) {
    display: none;
  }

  section > ul > li:nth-child(3) {
    margin: 0 auto .5rem 0;
  }

  section > ul > li:nth-child(4) {
    margin: 0 0 0 auto;
  }

  /* Hero Content Div */
  section > div {
    font-family: var(--font-text);
    font-weight: var(--font-light);
    color: var(--white);
    display: flex;
    justify-content: center;
    padding-top: 8rem;
    
    @media (min-width: 1024px) {
      padding-top: 3rem;
      justify-content: space-between;

      & > * {
        max-width: 30%;
      }
    }
  }
  
  /* Socials */
  section > div > ul {
    display: none;

    @media (min-width: 1024px) {
      font-weight: var(--font-medium);
      list-style-type: none;
      display: flex;
      align-items: center;
    }
    
  }
  
  section > div > ul > li:nth-child(2){
    display: flex;
    place-items: center;
    padding: 1rem;
    aspect-ratio: 1;

    background: var(--container-bg);
    width: fit-content;
    border-radius: 100%;
  }
  
  section > div > ul > li:nth-child(3){
    display: flex;
    place-items: center;
    padding: 1rem;
    aspect-ratio: 1;

    background: var(--container-bg);
    width: fit-content;
    border-radius: 100%;
  }

  /* About */

  section > div > article {
    display: none;
    @media (min-width: 1024px) {
      display: block;
    }
  }

  section > div > aside {
    position: relative;
		z-index: 5;
  }

  section > div > aside > button {
    position: relative;
		padding: 0.5rem 1rem;
		font-weight: 700;
		text-decoration: none;
		cursor: pointer;
    background: var(--cream-diagonal);
    color: var(--white);
    border-radius: var(--radius-btn);
    border: none;
    text-shadow: 0 0 .5rem rgba(0 0 0 0.25);
    font-family: var(--font-text);
    font-weight: var(--font-bold);
  }

  section > div > aside > button::before,
  section > div > aside > button::after {
    content: "";
    position: absolute;
    top: -3px;
    left: -3px;
    width: calc(100% + 6px);
    height: calc(100% + 6px);
    border-radius: var(--radius-btn-border);
  }
  
  section > div > aside > button::before {
    background: var(--silver-horizontal);
    z-index: -1;
  }
  
  section > div > aside > button::after {
    z-index: -2;
    filter: blur(10px);
    opacity: 50%;
    background: var(--cream-horizontal);
  }

</style>
