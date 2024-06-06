---
description: This page describes how to set up charging local taxes
---

# Local Tax Support

{% hint style="danger" %}
With the implementation of the new [Dashboard interface](https://docs.opencollective.com/help/product/understanding-your-dashboard), we are currently in the process of updating our documentation and some pages may be out of date. Thank you for your patience. Please [contact](https://opencollective.com/contact) our support team if you need any assistance.
{% endhint %}

In certain countries or regions, Fiscal Hosts are required to collect local taxes—for example, VAT in the EU.

Please [contact us](https://opencollective.com/contact) if you need Collectives under your umbrella to charge taxes. We will work with you to conform to your local legislation.

## VAT

{% hint style="warning" %}
VAT will only apply if the collective creates a `SERVICE` or `PRODUCT` tier and for events.
{% endhint %}

Once VAT is set up for a collective, we will start asking the country of residency and an optional VAT number to everyone who orders tiers or tickets from the collective. We will apply the VAT rules accordingly:

* Charge VAT from the country of the event if it's an event
* VAT percentage depends on the country where the collective is
* Don't charge VAT if a VAT number is provided and contribution comes from another EU country

### Enable VAT at the host level

If the host is the one supposed to collect VAT (most common case) then you can enable it by going to the Edit section (`https://opencollective.com/{my_host}/admin`) and set your country to a European country. The form will then ask for a VAT number.

![](<../.gitbook/assets/image (16) (2) (2) (1) (1).png>)

Your host is now ready to start accepting VAT. You still need to enable it on a per-collective basis by setting a country and a "VAT setting" for the collective on the collective edit page (`https://opencollective.com/{the_collective}/admin`).

### Enable VAT at the collective level

If the collective has a VAT number and should be responsible for collecting VAT itself, you can enable that by following the exact same steps as before, except that you'll choose the option `Use my own VAT number` on the last step.

![](<../.gitbook/assets/image (16) (1).png>)

## GST (New Zealand)

GST is also supported for New Zealand. [Contact us](https://opencollective.com/contact)!
