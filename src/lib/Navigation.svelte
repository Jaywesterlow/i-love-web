<script>
	import { Svg } from '$lib';
	import { onMount } from 'svelte';

	let showMenu = false;

	function toggleMenu() {
		showMenu = !showMenu;
		document.body.classList.toggle('no-scroll', showMenu);
	}

	function handleScroll() {
		const navbar = document.getElementById('navbar');
		if (window.scrollY > 50) {
			navbar.classList.add('sticky');
		} else {
			navbar.classList.remove('sticky');
		}
	}

	onMount(() => {
		window.addEventListener('scroll', handleScroll);
	});
</script>

<nav id="navbar">
	<ul>
		<li><Svg name="logo" /></li>
		<li><button id="menu-btn" on:click={toggleMenu}>MENU</button></li>
	</ul>
	<ul id="menu-content" class:menu-open={showMenu}>
		<li><a href="https://www.google.nl">Home</a></li>
		<li><a href="https://www.google.nl">Projects</a></li>
		<li><a href="https://www.google.nl">About me</a></li>
		<li><a href="https://www.google.nl">I Love Web</a></li>
		<li><a href="https://www.google.nl">Contact</a></li>
	</ul>
</nav>

<style>
  



	:global(body.no-scroll) {
      overflow: hidden;
      height: 100vh;
  }

	#navbar {
		width: 100%;
		position: sticky;
    top: 0;
		padding: 1rem 5% .5rem 5%;
		margin-bottom: -1px;
		font-family: var(--font-text);
		background: transparent;
		transition: 0.3s ease;
		z-index: 1000;
	}

	:global(#navbar.sticky) {
		position: fixed !important;
    transition: 0.3s ease !important;
    padding-top: .5rem !important;
    padding-bottom: .25rem !important;
	}

	@media (min-width: 1024px) {
		#navbar {
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
    background: var(--silver-diagonal);
    color: var(--white);
    border-radius: var(--radius-btn);
    border: none;
    text-shadow: 0 0 .5rem rgba(0 0 0 0.25);
	}

  nav ul:nth-child(1) button::before,
  nav ul:nth-child(1) button::after {
    content: "";
    position: absolute;
    top: -3px;
    left: -3px;
    background: var(--silver-horizontal);
    width: calc(100% + 6px);
    height: calc(100% + 6px);
    border-radius: var(--radius-btn-border);
    z-index: -1;
    box-shadow: 0 0 30px var(--silver-diagonal);
  }

  nav ul:nth-child(1) button::after {
    z-index: -2;
    filter: blur(10px);
    opacity: 50%;
  }

	nav ul:nth-child(2) {
		padding: 3rem 0;
		width: calc(100% + 2rem);
		height: 100vh;
		position: fixed;
		top: 0;
		right: calc(-3rem - 100%);
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-around;
		transition: 450ms cubic-bezier(0, 0.62, 0.57, 1.02);
		z-index: 2;
		font-size: 1rem;
		background-color: rgba(0, 0, 0, 0.75);

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
			background-color: transparent;
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
		content: '';
		position: absolute;
		bottom: 0;
		left: 0;
		width: 100%;
		height: 0.1em;
		background-color: var(--white);
		transition:
			opacity 300ms,
			transform 300ms;
		transform: translate3d(-101%, 0, 0);
		opacity: 1;
	}

	nav ul:nth-child(2) li a:hover::after,
	nav ul:nth-child(2) li a:focus::after {
		transform: translate3d(0, 0, 0);
	}
</style>
