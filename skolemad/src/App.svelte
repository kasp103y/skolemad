<script>
  export let name = "Slim Shady";
  import "carbon-components-svelte/css/all.css";
  import { Accordion, AccordionItem } from "carbon-components-svelte";
</script>

<main>
  <h1>Hi, my name is {name}</h1>
  <Accordion>
    <AccordionItem title="Natural Language Classifier">
      <p>
        Natural Language Classifier uses advanced natural language processing
        and machine learning techniques to create custom classification models.
        Users train their data and the service predicts the appropriate category
        for the inputted text.
      </p>
    </AccordionItem>
    <AccordionItem title="Natural Language Understanding">
      <p>
        Analyze text to extract meta-data from content such as concepts,
        entities, emotion, relations, sentiment and more.
      </p>
    </AccordionItem>
    <AccordionItem title="Language Translator">
      <p>
        Translate text, documents, and websites from one language to another.
        Create industry or region-specific translations via the service's
        customization capability.
      </p>
    </AccordionItem>
  </Accordion>
</main>
