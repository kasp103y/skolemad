<script>
  import Button from "./Button.svelte";
</script>

<section class="hero">
  <h1>SkoleMad</h1>
  <p class="p-lead">
    SkoleMad tilbyder en nem og fleksibel frokostordning til dine børn
  </p>
  <Button>Log ind/Opret bruger</Button>
</section>

<style>
  .hero {
    background-image: url("../barn-mad.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 90vh;
    background-position: 10% 37%;
    display: grid;
    justify-content: center;
    align-content: center;
  }
</style>
