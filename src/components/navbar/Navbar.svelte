<script>

</script>

<style>
  .navbar-menu .navbar-item {
    transition: all 0.3s ease-in-out;
    display: inline-block;
    height: 3.25rem;
    line-height: 3.25rem;
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
    height: 3.25rem;
  }

  .navbar-menu .navbar-item:hover:after {
    margin-top: -3.25rem !important;
  }

  .navbar-menu .navbar-item:hover {
    color: #1c234b !important;
    background-color: transparent !important;
  }
</style>

<nav
  class="navbar is-dark has-gradient-dark"
  role="navigation"
  aria-label="main navigation">
  <div class="container">
    <div class="navbar-brand">
      <a class="navbar-item" href="https://bulma.io">
        <img
          alt=""
          src="https://bulma.io/images/bulma-logo.png"
          width="112"
          height="28" />
      </a>
    </div>

    <div id="headerNavbar" class="navbar-menu">
      <div class="navbar-end">
        <a class="navbar-item" href="/">Home</a>
        <a class="navbar-item" href="/services">Services</a>
        <a class="navbar-item" href="/team">Team</a>
        <a class="navbar-item" href="/blog">Blog</a>
        <a class="navbar-item" href="/contact">Contact Us</a>
      </div>
    </div>
  </div>
</nav>
