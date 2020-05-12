<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Stripe Checkout Sample</title>
    <meta name="description" content="A demo of Stripe client-only Checkout" />

    <link rel="icon" href="favicon.ico" type="image/x-icon" />
    <link rel="stylesheet" href="css/normalize.css" />
    <link rel="stylesheet" href="css/global.css" />
    <!-- Load Stripe.js on your website. -->
    <script src="https://js.stripe.com/v3/"></script>
  </head>

  <body>
    <div class="sr-root">
      <div class="sr-main" style="display: flex;">
        <header class="sr-header">
          <div class="sr-header__logo"></div>
        </header>
        <div class="sr-container">
          <section class="container">
            <h1>One-time Donation</h1>
            <button
              data-checkout-mode="payment"
              data-price-id="sku_GU4JYXyvvRb2sX"
            >
              Donate $5.00 once
            </button>
            <button
              data-checkout-mode="payment"
              data-price-id="sku_GU4KO8nfdg8G2Z"
            >
              Donate $15.00 once
            </button>
            <button
              data-checkout-mode="payment"
              data-price-id="sku_GU4LB0wBViiYsm"
            >
              Donate $50.00 once
            </button>
          </section>
          <section class="container">
            <h1>Recurring Donation</h1>
            <button
              data-checkout-mode="subscription"
              data-price-id="plan_GU4MXg0k0Uv1S6"
            >
              Donate $20.00 per month
            </button>
          </section>
        </div>
        <div id="error-message"></div>
      </div>
    </div>
    <div class="banner">
      <span>
        This is a
        <a href="https://github.com/stripe-samples"> Stripe Sample </a> on how
        to use Stripe Checkout on GitHub Pages.
        <a
          href="https://github.com/stripe-samples/github-pages-stripe-checkout"
        >
          View code on GitHub.
        </a>
      </span>
    </div>

    <script>
      // Replace with your own publishable key: https://dashboard.stripe.com/test/apikeys
      var PUBLISHABLE_KEY = 'pk_test_Tr8olTkdFnnJVywwhNPHwnHK00HkHV4tnP';
      // Replace with the domain you want your users to be redirected back to after payment
      var DOMAIN = location.href.replace(/[^/]*$/, '');

      if (PUBLISHABLE_KEY === 'pk_test_Tr8olTkdFnnJVywwhNPHwnHK00HkHV4tnP') {
        console.log(
          'Replace the hardcoded publishable key with your own publishable key: https://dashboard.stripe.com/test/apikeys'
        );
      }

      var stripe = Stripe(PUBLISHABLE_KEY);

      // Handle any errors from Checkout
      var handleResult = function (result) {
        if (result.error) {
          var displayError = document.getElementById('error-message');
          displayError.textContent = result.error.message;
        }
      };

      document.querySelectorAll('button').forEach(function (button) {
        button.addEventListener('click', function (e) {
          var mode = e.target.dataset.checkoutMode;
          var priceId = e.target.dataset.priceId;
          var items = [{ price: priceId, quantity: 1 }];

          // Make the call to Stripe.js to redirect to the checkout page
          // with the sku or plan ID.
          stripe
            .redirectToCheckout({
              mode: mode,
              lineItems: items,
              successUrl:
                DOMAIN + 'success.html?session_id={CHECKOUT_SESSION_ID}',
              cancelUrl:
                DOMAIN + 'canceled.html?session_id={CHECKOUT_SESSION_ID}',
            })
            .then(handleResult);
        });
      });
    </script>
  </body>
</html>
