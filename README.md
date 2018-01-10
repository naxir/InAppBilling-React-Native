
**We can test the result with static responses, you can use reserved productids as defined by Google.**
There are four reserved product IDs for testing static In-app Billing responses:

**android.test.purchased**
When you make an In-app Billing request with this product ID, Google Play responds as though you successfully purchased an item. The response includes a JSON string, which contains fake purchase information (for example, a fake order ID).

**android.test.canceled**
When you make an In-app Billing request with this product ID Google Play responds as though the purchase was canceled. This can occur when an error is encountered in the order process, such as an invalid credit card, or when you cancel a user's order before it is charged.

**android.test.refunded**
When you make an In-app Billing request with this product ID, Google Play responds as though the purchase was refunded. Refunds cannot be initiated through Google Play's in-app billing service. Refunds must be initiated by you (the merchant). After you process a refund request through your Google payments merchant account, a refund message is sent to your application by Google Play. This occurs only when Google Play gets notification from Google payments that a refund has been made. For more information about refunds, see Handling IN_APP_NOTIFY messages and In-app Billing Pricing.

**android.test.item_unavailable**
When you make an In-app Billing request with this product ID, Google Play responds as though the item being purchased was not listed in your application's product list.




You can only test  in app billing result with fake product id's on real devices 
so please do not test it on emulator 
**Thanks** 
