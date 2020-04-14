<script>
  import { scrollto } from "svelte-scrollto";
</script>

<style>
  .navbar-menu .navbar-item {
    transition: all 0.3s ease-in-out;
    display: inline-block;
    height: 3.5rem;
    line-height: 3.5rem;
    position: relative;
    overflow: hidden;
    padding: 0;
    min-width: 100px;
    text-align: center;
  }

  .navbar-menu .navbar-item:before {
    transition: all 0.1s linear;
    content: attr(value);
    display: block;
  }

  .navbar-menu .navbar-item:after {
    transition: all 0.3s ease-in-out;
    content: "";
    display: block;
    background-color: #94fbb4;
    margin-top: 0px;
    height: 3.5rem;
  }

  .navbar-menu .navbar-item:hover:after {
    margin-top: -3.5rem !important;
  }

  .navbar-menu .navbar-item:hover {
    color: #1c234b !important;
    background-color: transparent !important;
  }

  .navbar-item img {
    max-height: 3rem;
  }
</style>

<nav
  id="navbar"
  class="navbar is-dark has-gradient-dark"
  role="navigation"
  aria-label="main navigation">
  <div class="container">
    <div class="navbar-brand">
      <a class="navbar-item" href="/">
        <img alt="" src="logo-dark.png" width="112" />
      </a>
    </div>

    <div id="headerNavbar" class="navbar-menu">
      <div class="navbar-end">
        <a class="navbar-item" href="/">Home</a>
        <a
          class="navbar-item"
          use:scrollto={{ element: '#services', offset: 0 }}
          href="·">
          Services
        </a>
        <a
          class="navbar-item"
          use:scrollto={{ element: '#team', offset: 0 }}
          href="·">
          Team
        </a>
        <a class="navbar-item" href="/dataviz">Data Viz</a>
        <a
          class="navbar-item"
          use:scrollto={{ element: '#contact', offset: 0 }}
          href="·">
          Contact Us
        </a>
      </div>
    </div>
  </div>
</nav>
