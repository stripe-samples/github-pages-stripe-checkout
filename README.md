# GitHub Payment Pages with Stripe Checkout

This is an example of a client-only (server-free) donation payment page that can be hosted on GitHub using Stripe Checkout.

## Setup

- Create Stripe Account: https://dashboard.stripe.com/register
- Enable client-only checkout: https://dashboard.stripe.com/account/checkout/settings
- Create a one-time or recurring product in the Stripe Dashboard: https://dashboard.stripe.com/products
  - After creation click the "Use with checkout" button and copy the sku (sku_xxx) or plan (plan_xxx) ID
  - Paste the IDs into the button `data-sku-id`/`data-plan-id` attributes.
- Copy your publishable key from: https://dashboard.stripe.com/apikeys and set it as the value for `PUBLISHABLE_KEY` in the index.html file

## Run locally

Since these are all static assets you can serve them locally with a simple web server, e.g.

    python -m SimpleHTTPServer 8888

You can now view your page at http://localhost:8888

## GitHub Pages Demo

See demo (in test mode) running here: https://thorsten-stripe.github.io/github-pages-stripe-checkout

## Go live

- Add `username.github.io` (replace username with your github user name) to the domain whitelist in https://dashboard.stripe.com/account/checkout/settings
- Replace the test publishable key `PUBLISHABLE_KEY` in the index.html file with your pk\*live_xxx key which can be found here: https://dashboard.stripe.com/test/apikeys (!!!**NOTE**!!!: never paste in your secret key! For client-only Checkout only the publishable key is needed!)
- Commit the changes to the `gh-pages` branch and push them to GitHub.
- Done, you can now accept live payments on your GitHub pages \o/
