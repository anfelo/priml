<script>
  import { scrollto } from "svelte-scrollto";
</script>

<style>
  .hero {
    position: relative;
  }

  .hero-body .title {
    padding-bottom: 10px;
    font-size: 8rem;
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

  .scroll-down-btn {
    display: none;
    position: absolute;
    bottom: -250px;
    left: 50%;
    transform: translateX(-50%);
    color: white;
    font-size: 2rem;
    -webkit-animation-duration: 1s;
    animation-duration: 1s;
    -webkit-animation-fill-mode: both;
    animation-fill-mode: both;
    -webkit-animation-timing-function: ease-in-out;
    animation-timing-function: ease-in-out;
    animation-iteration-count: infinite;
    -webkit-animation-iteration-count: infinite;
    z-index: 1;
  }

  .scroll-down-btn:hover {
    animation-name: bounce;
    -moz-animation-name: bounce;
  }

  @keyframes bounce {
    0%,
    100%,
    20%,
    50%,
    80% {
      -webkit-transform: translate(-50%, 0);
      -ms-transform: translate(-50%, 0);
      transform: translate(-50%, 0);
    }
    40% {
      -webkit-transform: translate(-50%, -30px);
      -ms-transform: translate(-50%, -30px);
      transform: translate(-50%, -30px);
    }
    60% {
      -webkit-transform: translate(-50%, -15px);
      -ms-transform: translate(-50%, -15px);
      transform: translate(-50%, -15px);
    }
  }
</style>

<section class="hero is-dark has-gradient-dark is-fullheight-with-navbar">
  <div class="hero-body has-text-centered">
    <div class="container">
      <p class="title">We are Priml</p>
      <h2 class="subtitle">Problem Solvers & Data Fanatics</h2>
      <div class="buttons is-centered">
        <a
          class="button is-medium is-danger"
          use:scrollto={{ element: '#services', offset: 0 }}
          href="·">
          <div class="button-label">Check our services</div>
        </a>
        <a
          href="."
          class="button is-medium is-primary"
          use:scrollto={{ element: '#about', offset: 0 }}>
          <div class="button-label">More about Priml</div>
        </a>
      </div>
      <a
        href="."
        use:scrollto={{ element: '#services', offset: 0 }}
        class="scroll-down-btn has-text-white">
        <i class="fas fa-arrow-down" />
      </a>
    </div>
  </div>
</section>
