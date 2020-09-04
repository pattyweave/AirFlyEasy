<script>
  import Product from "./Product.svelte";

</script>

<style>
  section {
    display: block;
    height: 10em;
    background-color: #922cf8;
  }

  .bold {
    font-weight: 900;
  }
</style>

<section>
  <div style="padding: 3.7em; text-align: center">
    <Product
      words={'Get 6 Weeks of Workouts'}
      price={'price_1HMKYcCaW8DiCMO8cBzyPrYc'} />
    <!-- <button
      class="btn-light btn-lg btn round"
      style="background-color: orange; border-color: orange;">
      <span class="bold">Get 6 weeks of workouts</span>
    </button> -->
  </div>
</section>
