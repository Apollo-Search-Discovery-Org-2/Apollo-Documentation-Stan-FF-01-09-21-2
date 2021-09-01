# Donation Completed

### 

## Javascript Code
```js
window.appEventData098 = window.appEventData098 || [];
appEventData098.push({
  "event": "Donation Completed",
    "donation": {
        "cardType": "<cardType>",
        "donationFrequency": "<donationFrequency>",
        "donationType": "<donationType>",
        "isCardRequested": "<isCardRequested>",
        "item": [
            {
                "donationAmount": "<donationAmount>",
                "donationID": "<donationID>"
            }
        ],
        "payment": [
            {
                "paymentMethod": "<paymentMethod>",
                "paymentSequence": "<paymentSequence>"
            }
        ],
        "profile": {
            "address": {
                "city": "<city>",
                "postalCode": "<postalCode>",
                "stateProvince": "<stateProvince>"
            }
        },
        "total": {
            "currency": "<currency>"
        },
        "transactionID": "<transactionID>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|cardType|string|Describes the type of card requested as part of a donation.|Electronic, Physical|||||||
|city|string|The mailing city associated with the donation payment. |Atlanta, New York, Los Angeles, Chicago|||||||
|currency|string|Currency of the donation payment. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|donationAmount|string|String representation of the donation amount. Positive. Up to two decimal places for cents. No currency symbol.|200.00, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|donationFrequency|string|Recurrence frequency of donation. |One Time, Monthly|||||||
|donationID|string|Unique identifier of the donation. Max Length 20. Used to prevent duplication.||^[a-zA-Z0-9]{6,20}$|6|20||||
|donationType|string|Type of donation selected. |Tribute, General, Fundraiser|||||||
|isCardRequested|boolean|Boolean flag indicating whether a card was requested as part of a donation.|TRUE, FALSE|||||||
|paymentMethod|string|Describes the method of payment for a transaction. |Credit Card, PayPal, Mastercard, Visa, Amex, Discover|||||||
|paymentSequence|integer|Integer indicator of the sequence in which payments were applied within a transaction.  Starting with 1.|1, 2, 3, 4, 5||||1|||
|postalCode|string|The mailing zip or postalcode associated with the donation payment. |53533, 30381, M1R 0E9, M3C 0C1|||||||
|stateProvince|string|The mailing state or province associated with the donation payment. |MO, GA, NB, ON|||||||
|transactionID|string|Unique identifier of the transaction. Max Length 20. Used as a key for upload of post transaction data. ||^[a-zA-Z0-9]{6,20}$|6|20||||



