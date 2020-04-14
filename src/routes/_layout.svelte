<script>
  import Navbar from "../components/navbar/Navbar.svelte";
  import Footer from "../components/footer/Footer.svelte";
</script>

<style lang="scss" global>
  @import "./style/global.scss";

  .title::selection,
  .subtitle::selection {
    background-color: $light-green;
  }

  .title::-moz-selection,
  .subtitle::-moz-selection {
    background-color: $light-green;
  }

  .title {
    font-family: $family-cursive;
  }

  .has-gradient-dark {
    background: rgb(2, 0, 36);
    background: linear-gradient(
      90deg,
      rgba(2, 0, 36, 1) 0%,
      rgba(28, 35, 75, 1) 70%
    );
  }
</style>

<Navbar />

<main>
  <slot />
</main>

<Footer />
