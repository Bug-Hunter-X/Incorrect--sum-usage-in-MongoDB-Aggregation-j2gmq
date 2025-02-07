# MongoDB Aggregation Error: Incorrect $sum Usage

This repository demonstrates a common error when using the `$sum` operator within a MongoDB aggregation pipeline. The error arises from providing a string literal instead of a field expression to the `$sum` operator.

## Problem

The provided aggregation pipeline attempts to sum values from the `otherField` but incorrectly uses a string in the `$sum` operator. This will result in an error.

## Solution

The solution corrects the `$sum` operator by providing the correct field expression (`$otherField`).

## How to reproduce:
1. Install MongoDB
2. Create a collection and insert documents.
3. Run the code in `bug.js` to observe the error.
4. Run the code in `bugSolution.js` for the corrected version.
