<script>
  import "carbon-components-svelte/css/all.css";
  import { Accordion, AccordionItem } from "carbon-components-svelte";
  import Hero from "./components/Hero.svelte";
  import Bestil from "./Bestil.svelte";
  import NavBar from "./NavBar.svelte";
  import Konto from "./Konto.svelte";
  let page = "front";
</script>

<NavBar>
  <a href="#/bestil" on:click={() => (page = "bestil")}>Bestil </a>
  <a href="#/konto" on:click={() => (page = "konto")}>Konto </a>
</NavBar>

{#if page === "bestil"}
  <Bestil />
{:else if page === "konto"}
  <Konto />
{/if}

<main>
  <Hero />
  <Accordion>
    <AccordionItem title="Kunden">
      <p>
        Natural Language Classifier uses advanced natural language processing
        and machine learning techniques to create custom classification models.
        Users train their data and the service predicts the appropriate category
        for the inputted text.
      </p>
    </AccordionItem>
    <AccordionItem title="Leverandøren">
      <p>
        Analyze text to extract meta-data from content such as concepts,
        entities, emotion, relations, sentiment and more.
      </p>
    </AccordionItem>
    <AccordionItem title="Modtageren">
      <p>
        Translate text, documents, and websites from one language to another.
        Create industry or region-specific translations via the service's
        customization capability.
      </p>
    </AccordionItem>
  </Accordion>
</main>
