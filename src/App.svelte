<script>
	export let name;

	import CardWrapper from "./CartComponents/CardWrapper.svelte";
	import Navbar from "./cartComponents/Navbar.svelte";
	import Checkout from "./CartComponents/Checkout.svelte";
	let nav = "home";
	function navHandler(event) {
	  nav = event.detail.option;
	}
  </script>
  
  <Navbar on:nav={navHandler} />
  {#if nav === 'home'}
	<CardWrapper />
  {:else}
	<Checkout />
  {/if}



<!-- In the code above, we imported all the required Svelte components for rendering to App.svelte file, which is the top-level component of our App. -->

