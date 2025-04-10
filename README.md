# Mobile Number Validation Library

This npm library provides country data validation functionality, allowing you to retrieve data related to phone number lengths by country code. This library is created with reference to @zene/mobile-number-validator for custom modifications and active updates.

## Installation

You can install the library via npm:

```bash
  npm install country-phone-num-data-lib
```

## Usage

```javascript
// Vanilla JS
const { getCountryDataByCode } = require("country-phone-num-data-lib");

// React usage
import { getCountryDataByCode } from "country-mobile-number-validator";

// Example usage:
const countryCode = 1; // United States
const countryData = getCountryDataByCode(countryCode);
console.log(countryData);
```

```javascript
{
  country: 'United States',
  phLengthMax: 10,
  phLengthMin: 10,
  phExample: '+1 xxx-166314'
}
```

## API Reference

#### getCountryDataByCode

```
getCountryDataByCode(countryCode: number): NumberValidationData
```

| Parameter     | Type     | Description                                                    |
| :------------ | :------- | :------------------------------------------------------------- |
| `countryCode` | `number` | **Required**. The numeric country code for the desired country |

#### NumberValidationData Interface

```
{
    country: string;
    phLengthMax: number |null;
    phLengthMin: number | null;
    phExample?: string | number;
}

```

## License

[MIT](https://choosealicense.com/licenses/mit/)
