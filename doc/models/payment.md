## Payment

Represents a payment processed by the Square API.

### Structure

`Payment`

### Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Optional | Unique ID for the payment. |
| `created_at` | `string` | Optional | Timestamp of when the payment was created, in RFC 3339 format. |
| `updated_at` | `string` | Optional | Timestamp of when the payment was last updated, in RFC 3339 format. |
| `amount_money` | [`Money`](/doc/models/money.md) | Optional | Represents an amount of money. `Money` fields can be signed or unsigned.<br>Fields that do not explicitly define whether they are signed or unsigned are<br>considered unsigned and can only hold positive amounts. For signed fields, the<br>sign of the value indicates the purpose of the money transfer. See<br>[Working with Monetary Amounts](https://developer.squareup.com/docs/build-basics/working-with-monetary-amounts)<br>for more information. |
| `tip_money` | [`Money`](/doc/models/money.md) | Optional | Represents an amount of money. `Money` fields can be signed or unsigned.<br>Fields that do not explicitly define whether they are signed or unsigned are<br>considered unsigned and can only hold positive amounts. For signed fields, the<br>sign of the value indicates the purpose of the money transfer. See<br>[Working with Monetary Amounts](https://developer.squareup.com/docs/build-basics/working-with-monetary-amounts)<br>for more information. |
| `total_money` | [`Money`](/doc/models/money.md) | Optional | Represents an amount of money. `Money` fields can be signed or unsigned.<br>Fields that do not explicitly define whether they are signed or unsigned are<br>considered unsigned and can only hold positive amounts. For signed fields, the<br>sign of the value indicates the purpose of the money transfer. See<br>[Working with Monetary Amounts](https://developer.squareup.com/docs/build-basics/working-with-monetary-amounts)<br>for more information. |
| `app_fee_money` | [`Money`](/doc/models/money.md) | Optional | Represents an amount of money. `Money` fields can be signed or unsigned.<br>Fields that do not explicitly define whether they are signed or unsigned are<br>considered unsigned and can only hold positive amounts. For signed fields, the<br>sign of the value indicates the purpose of the money transfer. See<br>[Working with Monetary Amounts](https://developer.squareup.com/docs/build-basics/working-with-monetary-amounts)<br>for more information. |
| `processing_fee` | [`List of Processing Fee`](/doc/models/processing-fee.md) | Optional | Processing fees and fee adjustments assessed by Square on this payment. |
| `refunded_money` | [`Money`](/doc/models/money.md) | Optional | Represents an amount of money. `Money` fields can be signed or unsigned.<br>Fields that do not explicitly define whether they are signed or unsigned are<br>considered unsigned and can only hold positive amounts. For signed fields, the<br>sign of the value indicates the purpose of the money transfer. See<br>[Working with Monetary Amounts](https://developer.squareup.com/docs/build-basics/working-with-monetary-amounts)<br>for more information. |
| `status` | `string` | Optional | Indicates whether the payment is `APPROVED`, `COMPLETED`, `CANCELED`, or `FAILED`. |
| `source_type` | `string` | Optional | The source type for this payment<br><br>Current values include:<br>`CARD` |
| `card_details` | [`Card Payment Details`](/doc/models/card-payment-details.md) | Optional | Reflects the current status of a card payment. |
| `location_id` | `string` | Optional | ID of the location associated with the payment. |
| `order_id` | `string` | Optional | ID of the order associated with this payment. |
| `reference_id` | `string` | Optional | An optional ID that associates this payment with an entity in<br>another system. |
| `customer_id` | `string` | Optional | An optional customer_id to be entered by the developer when creating a payment. |
| `employee_id` | `string` | Optional | An optional ID of the employee associated with taking this payment. |
| `refund_ids` | `List of string` | Optional | List of `refund_id`s identifying refunds for this payment. |
| `buyer_email_address` | `string` | Optional | The buyer's e-mail address |
| `billing_address` | [`Address`](/doc/models/address.md) | Optional | Represents a physical address. |
| `shipping_address` | [`Address`](/doc/models/address.md) | Optional | Represents a physical address. |
| `note` | `string` | Optional | An optional note to include when creating a payment |
| `statement_description_identifier` | `string` | Optional | Additional payment information that gets added on the customer's card statement<br>as part of the statement description.<br><br>Note that the statement_description_identifier may get truncated on the statement description<br>to fit the required information including the Square identifier (SQ *) and name of the<br>merchant taking the payment. |
| `receipt_number` | `string` | Optional | The payment's receipt number.<br>The field will be missing if a payment is CANCELED |
| `receipt_url` | `string` | Optional | The URL for the payment's receipt.<br>The field will only be populated for COMPLETED payments. |

### Example (as JSON)

```json
{
  "id": null,
  "created_at": null,
  "updated_at": null,
  "amount_money": null,
  "tip_money": null,
  "total_money": null,
  "app_fee_money": null,
  "processing_fee": null,
  "refunded_money": null,
  "status": null,
  "source_type": null,
  "card_details": null,
  "location_id": null,
  "order_id": null,
  "reference_id": null,
  "customer_id": null,
  "employee_id": null,
  "refund_ids": null,
  "buyer_email_address": null,
  "billing_address": null,
  "shipping_address": null,
  "note": null,
  "statement_description_identifier": null,
  "receipt_number": null,
  "receipt_url": null
}
```

