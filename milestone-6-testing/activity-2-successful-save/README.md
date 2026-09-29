# Activity 2 — Test Successful Save

## Objective

Verify that a High Impact Incident can be successfully saved when the required **Assigned To** field is populated.

## Test Procedure

1. Navigate to **Incident → Create New**.
2. Set **Impact** to `1 - High`.
3. Select a valid user in the **Assigned To** field.
4. Verify that **Urgency** is automatically set to `1 - High`.
5. Click **Submit**.
6. Verify that the Incident is successfully saved.

## Expected Result

The Incident should be saved successfully without displaying the Assigned To validation error when the Assigned To field is populated.

The High Impact behavior should also remain active:

- Impact should be `1 - High`.
- Urgency should automatically be `1 - High`.
- The configured UI Policy behavior should remain active.

## Actual Result

The test was successfully completed.

The Incident was saved successfully as:

**INC0010005**

The saved Incident showed:

- **Impact:** `1 - High`
- **Urgency:** `1 - High`
- **Assigned To:** `Beth Anglin`

No Assigned To validation error was displayed, confirming that the onSubmit Client Script allowed the record to be saved when the required field was populated.

## Result

**PASS — Activity 2 completed successfully.**

## Evidence

The screenshot in this folder shows the successfully saved Incident and the configured High Impact behavior.
