<script>
  import { loadStripe } from "@stripe/stripe-js";

  export let price;
  export let words;

  // Basic Checkout
  async function startCheckout() {
    const stripe = await loadStripe(
      "pk_test_51HMKToCaW8DiCMO81jf53y1WvwXhjck2a5yfLvfl2YFndo6iRndu4WmSBhWERoSvjC8v5wiYw17bMyXdDPeIdrJu00BRSZkw6V"
    );
    const { error } = await stripe
      .redirectToCheckout({
        lineItems: [
          {
            price: price, // Replace with the ID of your price
            quantity: 1,
          },
        ],
        mode: "payment",
        successUrl: "https://google.com",
        cancelUrl: "https://localhost:5000",
      })
      .then(function (result) {
        // If `redirectToCheckout` fails due to a browser or network
        // error, display the localized error message to your customer
        // using `result.error.message`.
        alert("our payment system is broken");
      });

    if (error) {
      alert("our payment system is broken!");
    }
  }
</script>

<style>
  .bold {
    font-weight: 900;
    color: black;
    font-size: medium;
  }

  button {
    width: 30vw;
    background-color: orange;
    border: none;
    min-height: 40px;
    border-radius: 10px;
  }
</style>

<section>
  <button
    on:click={startCheckout}>
    <span class="bold">{words}</span>
  </button>

  <!-- <button on:click={startCheckout}> Buy me ${amount / 100} </button> -->
</section>
