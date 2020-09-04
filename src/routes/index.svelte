<script>
  import Product from "../components/Product.svelte";
  import Divider from "../components/Divider.svelte";
  import Dunks from "../components/Dunks.svelte";
</script>

<style>
  h1,
  figure,
  p {
    text-align: center;
    margin: 0 auto;
  }

  h1 {
    font-size: 2.8em;
    text-transform: uppercase;
    font-weight: 700;
    margin: 0 0 0.5em 0;
  }

  img {
    width: 100%;
    max-width: 400px;
    margin: 0 0 1em 0;
  }

  p {
    margin: 1em auto;
  }

  @media (min-width: 480px) {
    h1 {
      font-size: 4em;
    }
  }

  .basic-grid {
    display: grid;
    grid-gap: 1rem;
    grid-template-areas:
      "logo logo right right right right"
      "logo logo right right right right"
      "logo logo right right right right"
      "logo logo right right right right";
    color: white;
  }

  section {
    background-color: black;
  }

  .card {
    width: 100px;
    height: 100px;
    background-color: violet;
    color: white;
    border-radius: 10px;
  }

  @media screen and (min-width: 20rem) {
    .container {
      display: none;
    }
  }

  @media screen and (min-width: 70rem) {
    .container {
      padding-top: 50px;
      display: inline;
    }
    .second {
      text-align: center;
    }
  }

  .second {
    padding-top: 75px;
    text-align: center;
  }
</style>

<svelte:head>
  <title>Sapper project template</title>
</svelte:head>

<section class="basic-grid">
  <div class="container">
    <img alt="logo" width="100px" src="whiteLogo.png" />
  </div>

  <div class="second">
    <h1 class="bold huge center">Jump Higher.</h1>
    <h1 class="bold huge center">Run Faster.</h1>
    <br />
    <h3>
      A 6-week athletic development program to take your game to the next level
      with videos designed for your phone.
    </h3>
    <br />
    <br />
    <div>
      <Product words={'Enroll Now'} price={'price_1HMKYcCaW8DiCMO8cBzyPrYc'} />
      <br />
      <br />
      <p>18 workouts</p>
      <p>Day by day instruction</p>
    </div>
  </div>
</section>

<Divider />

<Dunks />

<Divider />
