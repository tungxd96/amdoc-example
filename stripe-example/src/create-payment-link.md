# Create a Payment Link

Create a custom payment page without code. Use the Stripe Dashboard to create a payment link that you can share with your customers. Stripe redirects customers who open this link to a Stripe-hosted payment page.

## Get Started

Before you begin, decide what pricing model works best for you:

### Products or Subscriptions

Best for e-commerce or SaaS where you’re selling products for a fixed price.

### Customers Choose What to Pay

Best for donations, tipping, or pay-what-you-want. This pricing model currently doesn’t support recurring payments or recurring donations. Learn more about the requirements for accepting tips or donations.

## Products or Subscriptions

1. **In the Dashboard, open the Payment Links page and click New (or click the plus sign and select Payment link).**
2. **Fill out the payment details.**
3. _(Optional)_ Set a preset amount.
4. _(Optional)_ Set minimum and maximum payment amounts. By default, the maximum payment amount is 10,000.00 USD. Contact support to increase this limit.
5. **Click Create link.**

### Payment Links on Mobile

If you’re creating a product or subscription, use the Stripe Dashboard iOS app to create a payment link on your mobile device. In the app, go to Payments > Payment Links to create a payment link (or click the create icon and select Payment link). The iOS app doesn’t currently support creating links where your customers choose how much to pay.

## Configure Payment Methods

With Dynamic payment methods, Stripe displays the most relevant and compatible payment methods to your customers, including Apple Pay and Google Pay. Stripe enables certain payment methods for you by default. We might also enable additional payment methods after notifying you. Use the Dashboard to enable or disable payment methods at any time. Learn more about [supported payment methods](https://stripe.com/docs/payments/payment-methods) and different types of payment methods.

You can review what payment methods your customers see in the Dashboard by entering a transaction ID or setting an order amount and currency.
