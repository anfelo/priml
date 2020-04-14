<script>
  import Card from "../card/Card.svelte";

  export let sectionId;
</script>

<style>
  .section .title {
    font-size: 4rem;
    color: white;
  }

  .section .subtitle {
    color: white;
    max-width: 50%;
    margin: auto;
    padding-bottom: 20px;
  }
</style>

<section id={sectionId} class="section is-dark has-gradient-dark ">
  <div class="container has-text-white has-text-centered">
    <h1 class="title">What we do</h1>
    <h2 class="subtitle">
      At Priml, our goal is to help elevate teams - giving them the push they
      need to truly succeed in today's ever-changing tech world.
    </h2>

    <div class="columns">
      <div class="column">
        <Card />
      </div>
      <div class="column">
        <Card />
      </div>
      <div class="column">
        <Card />
      </div>
      <div class="column">
        <Card />
      </div>
    </div>
  </div>
</section>
