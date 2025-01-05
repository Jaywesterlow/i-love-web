<script>
	import { Svg } from '$lib';
</script>

<section>
	<h1>Jaymar Westerlow, Web designer- & Developer</h1>

  <ul>
    <li><img src="/portrait.png"/></li>
    <li><img src="/jvv.png"/></li>
    <li>WEB DESIGNER</li>
    <li>& DEVELOPER</li>
  </ul>

  <div>
    <ul>
      <li>CONNECT WITH ME:</li>
      <li><Svg name="instagram" /></li>
      <li><Svg name="linkedin" /></li>
    </ul>

    <article>
      <p>
        Hello, I’m <strong>Jaymar</strong> -I design and develop <strong>web-apps</strong> 
        and specialize in <strong>accessibility</strong> and <strong>performance</strong>. 
        <span>
          I focus on creating unique, memorable designs while maintaining <strong>clean</strong>, 
          <strong>professional</strong> standards.
        </span>
      </p>
    </article>
    <aside>
      <button>CONTACT ME</button>
    </aside>
  </div>
  <button></button>
</section>

<style>
  section {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: calc(100dvh - 87px);
    padding: 4rem 0 1rem;

    @media (min-width: 1024px) {
      height: calc(100dvh - 119px);
      padding: 12rem 0 1rem;
    }
    
    @media (min-width: 1440px) {
      padding: 14rem 0 1rem;
    }
  }
  
  section h1 {
    display: none;
  }

  /* Hero title */
  section > ul {
    font-family: var(--font-title);
    font-weight: var(--font-bold);
    color: var(--white);
    display: flex;
    gap: .5rem 1rem;
    flex-direction: column;
    align-items: center;
    font-size: 2rem;
    list-style-type: none;

    @media (min-width: 500px) {
      font-size: 2.5rem;
    }
    
    @media (min-width: 1024px) {
      font-size: 4rem;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: center;
    }
    
    @media (min-width: 1440px) {
      font-size: 5.5rem;
    }
  }

  section > ul > li {
    display: flex;
    align-items: center;
  }

  /* portrait image */
    section > ul > li:nth-child(1) {
    margin-bottom: 3rem;
    
    @media (min-width: 1024px) {
      order: 2;
      margin: 0;
      width: calc(34% - .5rem);
        
      & img {
        max-width: 6rem;
      }
    }
    
    @media (min-width: 1440px) {
      width: calc(30% - .5rem);
      
      & img {
        max-width: 8rem;
      }
    }
  }

  /* JVV logo */
  section > ul > li:nth-child(2) {
    display: none;
    
      @media (min-width: 1024px) {
        display: flex;
        align-items: center;
        justify-content: flex-end;
        order: 3;
        width: calc(35% - .5rem);
        
        & img {
          max-width: 6rem;
        }
      }

      @media (min-width: 1440px) {
        width: calc(30% - .5rem);
        & img {
          max-width: 7rem;
        }
      }
  }

  /* Web Designer */
  section > ul > li:nth-child(3) {
    margin: 0 0 .5rem -25%;

    @media (min-width: 1024px) {
      margin: 0;
      order: 1;
      width: calc(66% - .5rem);
      justify-content: flex-end;
    }

    @media (min-width: 1440px) {
      width: calc(70% - .5rem);
    }
  }

  /* & Developer */
  section > ul > li:nth-child(4) {
    margin: 0 -25% 0 0;
    
    @media (min-width: 1024px) {
      margin: 0;
      order: 4;
      width: calc(65% - .5rem);
      justify-content: flex-start;
    }

    @media (min-width: 1440px) {
      width: calc(70% - .5rem);
    }
    
    @media (min-width: 1440px) {
      width: calc(70% - .5rem);
    }
  }

  /* Hero Content Div */
  section > div {
    font-family: var(--font-text);
    font-weight: var(--font-light);
    color: var(--white);
    display: flex;
    justify-content: center;
    
    @media (min-width: 768px) {
      justify-content: space-around;
      padding-top: 4rem;

      & > * {
        max-width: 45%;
      }
    }

    @media (min-width: 1024px) {
      padding-top: 10rem;
      justify-content: space-between;

      & > * {
        max-width: 30%;
      }
    }

    @media (min-width: 1440px) {
      padding-top: 11rem;
    }
  }
  
  /* Socials */
  section > div > ul {
    display: none;

    @media (min-width: 768px) {
      font-weight: var(--font-medium);
      list-style-type: none;
      display: flex;
      align-items: center;
    }
  }
  
  section > div > ul > li:not(:last-child){
    margin: 0 1rem 0 0;
  }
  
  section > div > ul > li:nth-child(1) {
    min-width: 155px;
  }

  section > div > ul > li:nth-child(2),
  section > div > ul > li:nth-child(3) {
    display: flex;
    place-items: center;
    padding: .6rem;
    aspect-ratio: 1;
    background: var(--container-bg);
    width: fit-content;
    border-radius: 100%;

    @media (min-width: 1024px) {
      padding: .75rem;
    }
  }

  /* About */
  section > div > article {
    display: none;

    @media (min-width: 1024px) {
      display: block;
    }

    & p span {
      display: none;

      @media (min-width: 1300px) {
        display: inline;
      }
    }
  }

  /* Contact button */
  section > div > aside {
    position: relative;
    display: flex;
    align-items: center;
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

/* ----------------------------------------------------- */
  section > button {

  }

</style>
