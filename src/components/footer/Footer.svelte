<script>
  import { scrollto } from "svelte-scrollto";
</script>

<style>
  .footer {
    padding-bottom: 2rem;
  }
  .footer .title {
    width: 70%;
    font-size: 4rem;
    color: white;
  }

  .footer .subtitle {
    color: white;
    margin: auto;
    padding-bottom: 20px;
  }

  .footer a:hover {
    color: white;
  }

  .footer .button:hover {
    background-color: transparent;
  }

  .footer .button-label:after {
    border-color: #94fbb4;
  }

  .footer-bottom {
    margin-top: 10rem;
    color: #999;
  }

  .footer-bottom a {
    color: #999;
  }
</style>

<footer class="footer has-background-black">
  <div class="container">
    <div class="columns is-variable is-4">
      <div class="column">
        <h1 class="title has-text-white">Want to see what AI is capable of?</h1>
      </div>
      <div class="column is-4">
        <p class="subtitle">
          Drive your business decisions based on predictive analytics, Machine
          Learning and Neural Networks.
        </p>
        <a
          href="."
          class="button is-medium is-black"
          use:scrollto={{ element: '#contact', offset: 0 }}>
          <div class="button-label has-text-success">
            Learn more about Priml
          </div>
        </a>
      </div>
    </div>
    <div class="columns footer-bottom">
      <div class="column">
        <p>
          <small>© 2019-2020 Priml</small>
        </p>
      </div>
      <div class="column">
        <p class="has-text-right">
          <a href="." use:scrollto={{ element: '#navbar', offset: 0 }}>
            Back to Top &nbsp;
            <i class="fas fa-arrow-up" />
          </a>
        </p>
      </div>
    </div>
  </div>
</footer>
