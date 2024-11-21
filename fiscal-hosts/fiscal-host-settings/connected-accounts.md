---
description: >-
  You can connect social media accounts to automatically thank new financial
  contributors
---

# Connect external accounts

## Receiving contributions through PayPal

{% hint style="info" %}
This feature is currently in **beta**, meaning it's still being tested. To turn on PayPal contributions, [email support](mailto:support@opencollective.com).
{% endhint %}

### Fees

Payment processor fees charged by PayPal will be automatically deducted. If any platform tips or platform share is paid through PayPal, it will go to your account and will be paid later, via the monthly settlement expense.

### Connecting PayPal

If you're already in the beta test group, you can follow these instructions:

*   [ ] Create a new PayPal app

    * Open [PayPal's Developer](https://developer.paypal.com/developer/applications/) page and Log In.
    * In _My Apps & Credentials_ page, select the **Live** environment, and click in _Create app_.

    ![](<../../.gitbook/assets/image (34).png>)

    * Name this App after Open Collective, this way you'll always remember where this token is being used.
    * Click _Create App._

![](<../../.gitbook/assets/Screen record from 2020-07-10 13.30.21.gif>)

<figure><img src="../../.gitbook/assets/paypal-features.png" alt=""><figcaption><p>To receive contributions, enable "Accept payments" and "Transactions search"</p></figcaption></figure>

* [ ] Then scroll down to "Live App Settings" and make sure "**Accept payments"** and **"Payouts"** are checked
* [ ] Now, copy the necessary information to Open Collective.
  * Open a new tab and go to [Open Collective](https://www.opencollective.com).
  * Open your Host collective settings page and click in the _Receiving Money_ option in the menu.
  * Copy and paste _Client ID, Secret_ in the respective fields, leave Webhook ID empty.
  * Click _Connect PayPal._
