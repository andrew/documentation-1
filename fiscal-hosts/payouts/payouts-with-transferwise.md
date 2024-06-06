---
description: Instructions on how to safely connect to Wise, f.k.a. TransferWise.
---

# Payouts with Wise

{% hint style="danger" %}
With the implementation of the new [Dashboard interface](https://docs.opencollective.com/help/product/understanding-your-dashboard), we are currently in the process of updating our documentation and some pages may be out of date. Thank you for your patience. Please [contact](https://opencollective.com/contact) our support team if you need any assistance.
{% endhint %}

For hosts that are using Wise, this integration can be used to automate expense payment by providing a one-click solution for paying expenses.

After connecting your Wise account, users submitting new expenses will have access to a structured form for providing a valid bank account information and you will be able to pay those expenses automatically with the _Pay with Wise_ button.

## Fees

### What are the fees involved?

The fees are charged by Wise and its value will vary with the currencies and value being transferred. You can read more about [Wise fees here](https://transferwise.com/help/13/understanding-fees-and-rates/2522717/how-do-you-determine-your-fees).

### Who pays these fees?

These fees are paid by the collective the expense was submitted for. This means that transactions in Wise will display the fees but that value will also be deducted from the collective balance in our platform as a _payment processor fee_.

![An expense submitted to Open Collective Engineering paid using TransferWise.](<../../.gitbook/assets/image (67).png>)

## Limitations

* Payments through Wise require a borderless account.
* Payments should respect the fund amount you have accounted for in the platform.
  * You can't pay expenses if the budget accounted for the collective is not enough to cover the transfer expenses.
* The host is still responsible for managing funds in Wise.
  * Transfers are funded with your host currency.
    * If your host is using USD, we're funding all your transfers with your USD balance despite the payee currency.

## Connecting Wise

* Go to [Open Collective](https://www.opencollective.com).
* Open your Host collective settings page and click on the _Sending Money_ option in the menu. ![](<../../.gitbook/assets/Kapture 2020-05-13 at 10.15.15.gif>)  &#x20;
* Click on _Connect Wise_ button;

![](<../../.gitbook/assets/Screenshot from 2021-05-12 18-46-55.png>)

* Now, log in with your business's Owner account and, if requested, select your business profile;
* Click on the _Give Access_ button:

![](<../../.gitbook/assets/Screenshot from 2021-05-12 18-49-51.png>)

* Done! Now all your hosted collectives will be able to submit Bank Transfer expenses compatible with TransferWise and you'll be able to pay for it with one click.
  * Notice that this option will only be available for new expenses. Expenses created before Wise support was added are not structured as required by Wise and will need to be edited or recreated by the payee.

## Paying Expenses

Once you're connected to Wise and you start receiving expenses requesting a bank account transfer, you'll be able to automatically pay that from your main Wise balance with a single click. The _Go to Pay_ button in approved expenses displays the Wise icon and by clicking this button you'll open the _Pay expense_ modal.

![Approved Expense submitted with Bank account information.](<../../.gitbook/assets/Screenshot from 2021-06-29 16-25-08.png>)

In the _Pay expense_ modal you can select if you want to pay it automatically with the integration or pay it manually, effectively marking the expense as paid so you can use any other method you want to settle this expense.

![Pay expense modal set to pay the expense automatically.](<../../.gitbook/assets/Screenshot from 2021-06-29 16-23-02.png>)

### Batching and Paying expenses using OTT

For some accounts (especialy in Europe and UK), Wise will require you to authorize the payment using an One-Time Token sent to you through SMS, Email or the Wise app.

![You can schedule expenses to manually pay in batches when Wise requires OTT authorization.](<../../.gitbook/assets/Screenshot from 2021-06-29 16-11-03.png>)

On such case, _Pay expense_ modal displays the _Schedule to Pay with Wise_ button that once clicked marks the expense as _Scheduled for Payment_. This will allow you to batch multiple expense for payment and authorizing all the payments in a single transaction.

In order for paying for the scheduled expenses, the host admin can find the _Pay Batch_ button on a suspended banner in the expenses page in the host dashboard:

![](<../../.gitbook/assets/Screenshot from 2021-06-29 16-18-33.png>)

If you click on _Pay Batch_, a confirmation modal will be displayed and if you click _Pay with Wise,_ all scheduled expenses are going to be batched in a single Wise group transaction.

![](<../../.gitbook/assets/Screenshot from 2021-06-29 16-42-45.png>)

This batch will be automatically funded after you confirmthe transaction using the one-time token generated by Wise and sent to you.

![](<../../.gitbook/assets/Screenshot from 2021-06-29 11-29-34.png>)

## Reducing Risks

In order to reduce risks related to having an active API token that is able to create and fund transactions, we strongly suggest you to:

1. Activate the Two-Step Authentication in Wise.
2. Keep just enough balance in Wise to pay your expenses.
   * This can be achieved by calculating the amount needed for the current payment cycle and transferring it beforehand.

## Troubleshooting

* `Unable to fund transfer`
  * Double-check if you have enough funds in your Wise balance, you'll be using the balance with the same currency of your OpenCollective account.
