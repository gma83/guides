# VAT on checkout

Content:
-   [Configure VAT for features](Custom-fields-eu-vat.md#configure-vat-for-features)
    - [EU countries](https://docs.yclas.com/eu-vat/#eu-countries)
    - [Non EU countries](https://docs.yclas.com/eu-vat/#non-eu-countries)
-   [Configure VAT for sellers](https://docs.yclas.com/eu-vat/#configure-vat-for-sellers)
    - [Advertisement VAT number](https://docs.yclas.com/eu-vat/#advertisement-vat-number)
    -   [User VAT number](https://docs.yclas.com/eu-vat/#user-vat-number)
-   [The checkout page](https://docs.yclas.com/eu-vat/#the-checkout-page)
-   [VAT on automatic emails](https://docs.yclas.com/eu-vat/#vat-on-automatic-emails)
-   [VAT for non EU countries](https://docs.yclas.com/eu-vat/#vat-for-non-eu-countries)

This feature is available on our 3.0.0 release and for all the sites hosted at  [Yclas.com](https://yclas.com/)

Yclas allows you to include VAT to the orders. When users purchase Featured Ads, To Top, Pay to Post or Membership plans the VAT will be added at checkout. You can also configure your website in a way where users can enter their VAT number and the VAT will be added automatically at the checkout when they are selling their products.

## Configure VAT for features

Follow the steps below to add the VAT to the features of your website,  **Featured Ads**,  **To Top**,  **Pay to Post**  and  **Membership plans**.

### EU countries

1.  Login to your panel.
2.  Go to  **Settings -> Payment -> General**.
3.  Enter the  **VAT country**  and  **VAT number**.
4.  Click  **Save**.

Once you click Save you should get a success message. If you get the following message it means that VAT country or number is wrong :

_Error: Invalid EU Vat Number, please verify number and country match_

### Non EU countries

1.  Login to your panel.
2.  Go to  **Settings -> Payment -> General**.
3.  Enter the  **VAT country**,  **VAT number**  and  **VAT rate only for Non-EU countries**.
4.  Click  **Save**.

## Configure VAT for sellers

If you don’t know how to enable the Buy Now button,  [here’s how](https://docs.yclas.com/pay-directly-from-ad/#how-to-activate-buy-now-button).

Sellers can enter their VAT number and include VAT at checkout when they are selling their products through your website. This can be done in two ways: using  [Advertisement Custom Fields](https://docs.yclas.com/how-to-create-custom-fields/)  or  [User Custom Fields](https://docs.yclas.com/users-custom-fields/).

At checkout, your website will try to calculate the VAT using the Advertisement VAT number, if it’s missing it will use the User VAT number and if that is missing too, then no VAT will be added on the amount.

### Advertisement VAT number

1.  Login to your panel.
2.  Go to  **Classifieds -> Custom Fields**.
3.  Click  **New Field**.
4.  Enter  **vatcountry**  into the field called Name. It’s important to enter  _vatcountry_  as name and choose Country as the field type in order to make the feature works. Choosing Country will automatically create dropdown menu with all the countries included.
5.  **Fill the fields**  and  **press Create**.
6.  Click  **New Field**.
7.  Enter  **vatnumber**  into the field called “Name”. It’s important to enter  _vatnumber_  as name in order to make the feature works.




### User VAT number

1.  Login to your panel.
2.  Go to  **Users -> User Custom Fields**.
3.  Click  **New Field**.
4.  Enter  **vatcountry**  into the field called “Name”. It’s important to enter  _vatcountry_  as name and choose Country as the field type in order to make the feature works. Choosing “Country” will automatically create dropdown menu with all the countries included.
5.  **Fill the fields**  and  **press Create**.
6.  Click  **New Field**.
7.  Enter  **vatnumber**  into the field called “Name”. It’s important to enter  _vatnumber_  as name in order to make the feature works.


## The checkout page

If the VAT country and the VAT number match, the checkout page will look like this.

## VAT on automatic emails

Once you configure VAT to be added at checkout, you will be able to include it to the **automatic emails**  _ads-sold_  and  _ads-purchased_.

The variables you can use are:

-   **[VAT.COUNTRY]**

Includes the two-letter country code.

-   **[VAT.NUMBER]**

Includes the VAT number.

-   **[VAT.PERCENTAGE]**

The VAT rate based on the seller VAT number.

## VAT for non EU countries

If your selected country is an EU member, the VAT rate is calculated automatically. The solution we have for non EU countries is for the seller to add manually the VAT rate, in his user profile details or each ad details.

To let sellers manually insert the VAT rate, you need to create a custom field or user custom field called  **vatnoneu**.

1.  Login to your panel.
2.  Go to  **Classifieds -> Custom Fields**  or  **Users -> User Custom Fields**.
3.  Click  **New Field**.
4.  Enter  **vatnoneu**  into the field called Name. It’s important to enter  _vatnoneu_  as name and choose Number Decimal in the field type to make this feature work.
5.  **Fill the fields**  and  **press Create**.