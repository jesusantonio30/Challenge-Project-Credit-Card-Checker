# Credit Card Validator

This project provides a set of ES6 JavaScript functions to validate credit card numbers, identify invalid ones, and determine the issuing companies of invalid cards. It is useful for detecting and categorizing invalid credit card numbers in datasets.

## Features

1. Validate credit card numbers using the Luhn algorithm.
2. Identify invalid credit cards from a batch of numbers.
3. Detect the issuing companies (e.g., Visa, Mastercard, etc.) associated with invalid credit cards.

## Usage

This project is designed to work with arrays of credit card numbers represented as arrays of digits. Use the provided functions to validate, filter, and categorize credit card numbers.

## Functions Overview

### `validateCred()`

Validates a single credit card number using the Luhn algorithm.

+ **Input**: An array of numbers representing a credit card.
+ **Output**: `"Valid"` if the card is valid, `"Invalid"` otherwise.

#### Example:
```javascript
validateCred([4, 5, 3, 9, 6, 7, 7, 9, 0, 8, 0, 1, 6, 8, 0, 8]);
// Output: "Valid"
```

### `idInvalidCardCompanies()`
  Identifies the companies associated with invalid credit card numbers.
  
+ Input: An array of invalid credit card numbers.
+ Output: An array of company names.
+ Supported Companies:
+ Amex (starting digit: 3)
+ Visa (starting digit: 4)
+ Mastercard (starting digit: 5)
+ Discover (starting digit: 6)

#### Example:
```javascript
      idInvalidCardCompanies([[3, 4, 4, 8, ...], [5, 3, 8, 2, ...]]); // Output: ["Amex", "Mastercard"]
```

## Dataset
Valid Credit Cards
```javascript
const valid1 = [4, 5, 3, 9, 6, 7, 7, 9, 0, 8, 0, 1, 6, 8, 0, 8];
const valid2 = [5, 5, 3, 5, 7, 6, 6, 7, 6, 8, 7, 5, 1, 4, 3, 9];
    // And so on...
```
    
Invalid Credit Cards
```javascript
const invalid1 = [4, 5, 3, 2, 7, 7, 8, 7, 7, 1, 0, 9, 1, 7, 9, 5];
const invalid2 = [5, 7, 9, 5, 5, 9, 3, 3, 9, 2, 1, 3, 4, 6, 4, 3];
    // And so on...
```

## Technologies Used
+ Language: JavaScript (ES6+)

Date: 1/25/2025



