# Payment methods

You must set up payment methods before you can open an order cycle.

## Accessing payment methods

Click **Enterprises **in the blue horizontal menu, and then click **Manage **next to your enterprise. Then, click Payment methods in the menu on the left hand side.

![](/assets/28-PaymentMethods2-1-Access-demo-farm_old.png)

## Creating a new payment method

![](/assets/28-PaymentMethods2-2-New-Payment-Method-Form_old.png)

The first step in setting up a Payment Method is to tick your enterprise, in the box on the right hand side of the page titled Hubs.  This indicates that the payment method you are about to create will apply to your enterprise.

**Name:** Choose a name for this payment method. \(i.e. PayPal, Cash on delivery, Bank Transfer, EFTPOS, etc\). It will be displayed at check out and on order confirmation emails.

**Description:** Here you can provide further details of the payment method. For instance, for a bank transfer, you would need to provide details of the bank account and request that customers provide you with the receipt number following payment. This description will be displayed at checkout and in order confirmation emails. An example of a description message displayed at checkout is shown below. The customer has selected ‘cash on collection/delivery’ and the ‘correct change…’ note is displayed.

![](/assets/28-PaymentMethods2-3-Payment-at-checkout_old.png)

**Active: **This field allows you to select whether this payment method will be currently visible and available.

**Active: **This field allows you to select whether this payment method will be currently visible and available.

**Tags:** Using tag rules you can make certain payment methods available for specific customers. See here for detail.

**Provider: **There are four provider options. Select the one which is relevant to the payment method you are creating.

1. MasterCard Internet Gateway Service \(MIGS\)
2. PayPal Express
3. [Pin Payments](https://pin.net.au/)
4. Cash/EFT/etc. \(this is for payments which do not require automatic validation\)

If you have selected ‘Cash/EFT/etc..’ as the provider, click **Create** to end the process.

For MasterCard, PayPal and Pin Payments additional instructions are below.

### PayPal

To setup a PayPal payment method, you need a PayPal business or merchant account. You can create one [here](/payment-methods.md). Once you have that, you can set up ‘API access’ within PayPal, which will enable FFW to connect customers directly with your PayPal account.

1. Login to your PayPal Account

2. Click Tools and then select API credentials

![](/assets/28-PaymentMethods2-4-Paypal-tools-API-credentials_old.png)

1. Click on ‘View API Signature’  and you will see the API details you’ll need to set up PayPal in FFW.

![](/assets/28-PaymentMethods2-5-API-Access_old.png)

![](/assets/28-PaymentMethods2-6-Api-Signature_old.png)

1. In FFW, make sure you are logged in as your Enterprise User. Go to an Enterprise and create a Payment Method. Select PayPal and fill in the details from the PayPal site.

**Login:**Type the API Username.

**Password:**Type the API Password.

**Signature:**Type the Signature  in this field.

![](/assets/28-PaymentMethods2-7-New-Payment-Paypal-1_old.png)

**Server**

Change the ‘server’ field to ‘live’ – this is case sensitive.

**Solution**

Solution determines whether or not a user needs a PayPal account to check out.

Type “Mark” if you do want users to have a PayPal account, or “Sole” if they can checkout without a PayPal account \(with credit card\).

**Landing Page**

You can select which page to show customers once they’re redirected to PayPal.

Type “Login” to direct customer to the login form for PayPal \(if you selected “Mark” above\). Or type “Billing” to show show customers a form where they can enter their credit card data and possibly sign up for a PayPal account \(if you selected “Sole” above\).

### MasterCard Internet Gateway Service \(MIGS\)

Set up of this service needs to be done through your bank.

### Pin Payments

For Pin Payments you only require your API key. You need to set up an account with Pin Payments first.

**API Key: **Enter your “Live Secret API Key’ here – you can find this in your PinPayments account \(see below\). First from your account, select API Keys. Then once you have generated an API key, copy the ‘Live Secret API Key’ and paste it into the API key field in FFW.



![](/assets/28-PaymentMethods2-8-API-Keys_old.png)

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-2.png "API 2")**Server:**Type ‘live’ – this is case sensitive.

## Fees on Payment Methods

[![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Calculator.png "Calculator")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Calculator.png)

You can attach a fee to payment methods. Most commonly this is used to pass on a payment fee to the customer, such as the PayPal charge. First you should select a fee calculator, then enter the value. A full description of the various fee calculators is below.

Note: Payment method fees do not include tax.

#### Fee Calculators

**Flat Percent **– This fee is charged as a percentage of the total amount charged in the order.

**Flat Rate \(per order\)**– This fee is applied as standard fee to all orders, regardless of the size of the order.

**Flexible Rate**– This calculator is typically used for promotional discounts where you charge a reduced fee as the customer makes more purchases of that item. This fee applies to items and products listed per kg or L.

* ‘First Item Cost’: The fee charged for the first item in the order.
* ‘Additional Item Cost’: The fee charged for additional items beyond the first.
* ‘Max Items’: The maximum number of items on which the fee will be applied. Items purchased beyond this amount will be not be charged the fee.

For example: If the first cost is $2, Additional Item Cost is $1 and the maximum items is three. If a customer orders 5 of the item, they will be charged $2 for the first item, $1 for the second and third, and no fee for the fourth and fifth.

**Flat Rate \(per item\)**–  This fee is a constant fee, applied to products listed as ‘items’. \(it will not be applied to products listed as per lb, or per gal\)

**Price Sack**– This fee is used to charge a discount on fees for orders which exceed a certain dollar amount.

* ‘Minimum Amount’: If the order’s total is below this amount, they will be charged the ‘Normal Amount’.
* ‘Discount Amount’: Orders which are equal to or greater than the minimum amount will be charged the ‘Discount Amount’.



