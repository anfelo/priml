<script>
  import Particles from "../components/particles/Particles.svelte";
</script>

<style>
  .hero-body .title {
    padding-bottom: 10px;
    font-size: 8rem;
    text-decoration: underline;
    text-decoration-color: #94fbb4;
  }

  .hero-body .buttons {
    position: absolute;
    left: 50%;
    width: 100%;
    transform: translateX(-50%);
    margin-top: 60px;
    z-index: 1;
  }

  .hero-body .container {
    margin-bottom: 100px;
  }
</style>

<svelte:head>
  <title>Priml | Home</title>
</svelte:head>

<section class="hero is-dark has-gradient-dark is-fullheight-with-navbar">
  <div class="hero-body has-text-centered">
    <div class="container">
      <p class="title">We are Priml</p>
      <h2 class="subtitle">Problem Solvers & Data Fanatics</h2>
      <div class="buttons is-centered">
        <a href="/services" class="button is-medium is-danger">
          <div class="button-label">Check our services</div>
        </a>
        <a href="/about" class="button is-medium is-primary">
          <div class="button-label">More about Priml</div>
        </a>
      </div>
    </div>
  </div>
</section>

<Particles />
