<script>
	import { Svg } from '$lib';

	let showMenu = false;

function toggleMenu() {
  showMenu = !showMenu;
  document.body.classList.toggle('no-scroll', showMenu);
}

</script>

<nav>
	<ul>
		<li><Svg name="arrow" /></li>
		<li><button id="menu-btn" on:click={toggleMenu}>MENU</button></li>
	</ul>
	<ul id="menu-content" class:menu-open={showMenu}>
		<li><a href="#">Home</a></li>
		<li><a href="#">Projects</a></li>
		<li><a href="#">About me</a></li>
		<li><a href="https://www.google.nl">I Love Web</a></li>
		<li><a href="#">Contact</a></li>
	</ul>
</nav>

<style>
body.no-scroll {
  overflow: hidden;
  height: 100vh;
}

nav {
  width: 100%;
  position: relative;
  padding: 1rem 5% 0 5%;
  margin-bottom: -1px;
  font-family: var(--font-text);

  @media (min-width: 1024px) {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1rem 10% 0 10%;
  }
}

nav ul:nth-child(1) {
  list-style-type: none;
  display: flex;
  justify-content: space-between;
  align-items: center;

  @media (min-width: 1024px) {
    width: 25%;
    justify-content: start;
  }
}

nav ul:nth-child(1) li:nth-child(2) {
  z-index: 5;

  @media (min-width: 1024px) {
    display: none;
  }
}

nav ul:nth-child(1) button {
  position: relative;
  padding: 0.5rem 1rem;
  font-weight: 700;
  text-decoration: none;
  cursor: pointer;
}

nav ul:nth-child(2) {
  padding: 3rem 0;
  width: calc(100% + 2rem);
  height: 100vh;
  position: absolute;
  top: 0;
  right: calc(-3rem - 100%);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  transition: 450ms cubic-bezier(0, 0.62, 0.57, 1.02);
  z-index: 2;
  font-size: 1rem;
  background-color: rgba(0, 0, 0, 0.8);

  @media (min-width: 1024px) {
    position: relative;
    top: auto;
    right: auto;
    flex-direction: row;
    justify-content: space-between;
    height: 100%;
    width: 75%;
    padding: 2rem 0 2rem 16%;
    font-size: 0.9rem;
  }

  @media (min-width: 1440px) {
    font-size: 1rem;
    padding: 2rem 0 2rem 28%;
  }
}

nav ul:nth-child(2).menu-open {
  right: -1rem;
}

nav ul:nth-child(2) li {
  transition: 300ms;
  list-style-type: none;
}

nav ul:nth-child(2) li a {
  display: block;
  position: relative;
  transition: 300ms;
  text-decoration: none;
  color: var(--white);
  overflow: hidden;

  @media (min-width: 1024px) {
    padding: 0.5rem 1rem;
  }
}

nav ul:nth-child(2) li a::after {
  content: "" ;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 0.1em;
  background-color: var(--white);
  transition: opacity 300ms, transform 300ms;
  transform: translate3d(-101%, 0, 0);
  opacity: 1;
}

nav ul:nth-child(2) li a:hover::after,
nav ul:nth-child(2) li a:focus::after{
  transform: translate3d(0, 0, 0);
}

</style>
