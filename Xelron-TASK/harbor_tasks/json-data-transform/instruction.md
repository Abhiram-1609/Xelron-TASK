# JSON Data Transformation Task

## Objective
You are assigned to write a script that processes an input JSON file and computes an aggregated sum based on specific criteria. The input data represents a list of transaction records.

## Requirements
- Read the input JSON file located at `/app/input.json`.
- Each record in the JSON has an `id`, `status` (a string), and `amount` (a number).
- Filter the list of records to include only those where the `status` is exactly "completed".
- Calculate the total sum of `amount` for these filtered "completed" records.
- Write the final calculation to a new JSON file located at `/app/output.json`.
- The output file must contain exactly this JSON structure:
```json
{
  "total_completed_amount": <total_sum_value>
}
```
- Ensure that you calculate this total dynamically by processing the input data; do not hardcode the expected answer.
- The output amount should be formatted or outputted as a regular JSON number.
