```markdown
# Track a Payment Link

Use URL parameters and UTM codes to track a payment link. Modify your payment link with URL parameters and Urchin Tracking Module (UTM) codes to get insight into customer behaviors and your marketing strategy’s effectiveness. These tools help identify the source of your traffic and the marketing campaigns leading to the most conversions.

## Track Campaigns with UTM Codes

Use UTM codes to track how customers find your site when they pay using your payment link. You can add the following UTM codes as parameters in the query string of your URL:

| PARAMETER    | DESCRIPTION                                                                                                                         |
| ------------ | ----------------------------------------------------------------------------------------------------------------------------------- |
| utm_source   | Identifies where the traffic originated (for example, a website name, social media, or a search engine).                            |
| utm_content  | Identifies what content your customer chooses. Use this parameter to distinguish between links that point to the same payment page. |
| utm_medium   | Identifies the marketing medium that accesses your payment link (for example, email, cost per click (cpc), or other methods).       |
| utm_term     | Identifies specific search terms and keywords in your paid search ads.                                                              |
| utm_campaign | Identifies your marketing campaigns using the payment link URL.                                                                     |

To add UTM codes, specify redirect as your confirmation behavior. When customers complete a payment, your redirect URL contains the UTM code parameters specified in your payment link URL. Here’s what a payment link looks like with appended UTM codes:
```

https://buy.stripe.com/test_eVa5nPg1j1wmfXq5kr?utm_medium=earned_email&utm_source=marketo&utm_campaign=campaign_a

```

### Caution

Construct UTM codes using alphanumeric characters, dashes, or underscores, ensuring they don’t exceed a 150-character limit. Invalid values are discreetly discarded, guaranteeing your payment links' performance remains unaffected.

## Simplify Reconciliation with a URL Parameter

You can simplify reconciliation with the `client_reference_id` URL parameter. Use URL parameters in the query string of your payment link URL. To configure URL parameters directly in the Dashboard Payment Links page:

1. Click the payment link you want to modify.
2. Click the down arrow of the Copy button and select URL parameters.
3. In the dialog, use the drop-down menu to select Client reference ID.
4. Enter a value that meets the requirements described in the following table to append the reference to your URL.
5. Copy the amended URL for use in your integration.

| PARAMETER           | DESCRIPTION                                                                                                                                                                               | SYNTAX                                                                                                                                                          |
|---------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client_reference_id | Use `client_reference_id` to attach a unique string of your choice to the Checkout Session. This can be a customer ID or a cart ID (or similar), and you can use it to reconcile the Session with your internal systems. If you add this parameter to your payment link, it’s sent in the `checkout.session.completed` webhook after payment completion. | `client_reference_id` can be composed of alphanumeric characters, dashes, or underscores, and be any value up to 200 characters. Invalid values are silently dropped, but your payment page continues to work as expected. |

```
