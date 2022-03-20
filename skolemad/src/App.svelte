<script>
  import "carbon-components-svelte/css/all.css";
  import { Accordion, AccordionItem } from "carbon-components-svelte";
  import Hero from "./components/Hero.svelte";

  import Button from "./components/Button.svelte";
  import Bestil from "./Bestil.svelte";
  import NavBar from "./NavBar.svelte";
  import Konto from "./Konto.svelte";
  let page = "front";
</script>

<NavBar>
  <a href="#/bestil" on:click={() => (page = "bestil")}>Bestil </a>
  <a href="#/konto" on:click={() => (page = "konto")}>Konto </a>
</NavBar>
<h1>Hallo {page}!</h1>

{#if page === "bestil"}
  <Bestil />
{:else if page === "konto"}
  <Konto />
{/if}
