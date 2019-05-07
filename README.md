# ![LOGO](logo.png) Brex **flow**ground Connector

## Description

A generated **flow**ground connector for the Brex API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/brex.io/1.0.0/openapi.json<br/>
Generated at: 2019-05-07T17:39:49+03:00

## API Description



## Authorization

Supported authorization schemes:
- API Key
## Actions

### Search announcements by id

*Tags:* `v1-company`

#### Input Parameters
* `id` - _required_ - announcement hex ID

### Deep Search (Search on register) by country and name

*Tags:* `v1-company`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars
* `name` - _required_ - company name

### Deep Search (Search on register) by country and register number.

*Tags:* `v1-company`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars
* `number` - _required_ - company registration number

### Search by country and name

*Tags:* `v1-company`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars
* `name` - _required_ - company name
* `limit` - _optional_ - number of search results

### Search by country and registration number

*Tags:* `v1-company`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars
* `number` - _required_ - company registration number
* `limit` - _optional_ - number of search results

### Search by country and mixed parameters. This function requires a country code then a mixture of name, number, url, phone, and vat. 0 or 1 of each parameter can be supplied. These are applied in a progressive filter mechanism in the order they are supplied (when properly implemented). This means it is possible to return empty sets when a later match returns an empty set.

*Tags:* `v1-company`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars

### Search announcements by company id

*Tags:* `v1-company`

#### Input Parameters
* `id` - _required_ - company hex ID

### Search announcements by company id

*Tags:* `v1-company`

#### Input Parameters
* `id` - _required_ - company hex ID

### Search for company superdata by id from previous call

*Tags:* `v1-company`

#### Input Parameters
* `id` - _required_ - company superdata by id
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars

### Search for company by id from previous call

*Tags:* `v1-company`

#### Input Parameters
* `id` - _required_ - company master data by id
* `dataset` - _required_ - company master data by id
    Possible values: , mini, master, full, refresh.

### Basic verification of given portuguese NIF number against NIF.com. Optional parameters may help to build a better confidence score.

*Tags:* `v1-nif-verification`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars

### Comprehensive verification of given portuguese NIF number against NIF.com. Optional parameters may help to build a better confidence score.

*Tags:* `v1-nif-verification`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars

### Order a new Pep Sanction Check

*Tags:* `v1-pepsanction`

#### Input Parameters
* `type` - _required_ - Type (Business or Person) of the requested Pep Sanction Check
    Possible values: , B, P.
* `search` - _required_ - Search string for the Pep Sanction Check

### Retrieve a delivered Pep Sanction check structured or in pdf

*Tags:* `v1-pepsanction`

#### Input Parameters
* `accept` - _optional_ - The type (pdf or json) in which the check should be returned
    Possible values: application/json, application/pdf.
* `id` - _required_ - The id of the ordered Pep Sanction Check (id as returned by orderPepSanction call)

### Check availabilty and valid options for a particular product for a particular subject

*Tags:* `v1-product`

#### Input Parameters
* `sku` - _required_ - SKU - 9 character value from a Product object
* `subjectId` - _required_ - Subject (e.g. Company) ID - 32 character hex value

### Return the current status of an existing notifier

*Tags:* `v1-product`

#### Input Parameters
* `notifierId` - _required_ - ID of the ProductOrderNotifier as returned from a /notifier POST call - 32 character hex value

### Place an order for a particular product for a particular subject

*Tags:* `v1-product`

#### Input Parameters
* `sku` - _required_ - SKU - 9 character value from a Product object
* `option` - _required_ - Product option (e.g. Accounts year) from a previous Availability call
* `subjectId` - _required_ - Subject (e.g. Company) ID - 32 character hex value

### Place an order for a particular product for a particular subject

*Tags:* `v1-product`

#### Input Parameters
* `sku` - _required_ - SKU - 9 character value from a Product object
* `subjectId` - _required_ - Subject (e.g. Company) ID - 32 character hex value

### Search for possible products for a particular subject

*Tags:* `v1-product`

#### Input Parameters
* `subjectId` - _required_ - Subject (e.g. Company) ID - 32 character hex value

### Get the status of an ongoing order

*Tags:* `v1-product`

#### Input Parameters
* `orderId` - _required_ - ID of the ProductOrder as returned from a /product/buy call - 32 character hex value

### Retrieves the document associated with a completed order

*Tags:* `v1-product`

#### Input Parameters
* `orderId` - _required_ - ID of the ProductOrder as returned from a /product/buy call - 32 character hex value

### Search for possible products for a particular subject

*Tags:* `v1-system`

### Retrieve pricing rules for your subscription plan

*Tags:* `v1-system`

### Basic verification of given VAT number against VIES. Optional parameters may help to build a better confidence score.

*Tags:* `v1-vat-verification`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars

### Extended verification of given VAT number against VIES and register. Optional parameters may help to build a better confidence score.

*Tags:* `v1-vat-verification`

#### Input Parameters
* `country` - _required_ - ISO_3166-1_alpha-2 representation of a country name - 2 chars

## License

**flow**ground :- Telekom iPaaS / brex-io-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
