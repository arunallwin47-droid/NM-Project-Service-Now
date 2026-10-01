# Activity 5 — Form-Based Update

## Objective

Verify that the Incident State can be changed successfully through the Incident form.

## Test Procedure

1. Open the same Incident record used in the previous tests.
2. Open the Incident form.
3. Change the **State** field to a new value.
4. Click **Update** to save the record.
5. Verify that the new State value is saved successfully.
6. Confirm that other configured fields continue to follow the UI Policy and Client Script rules.

## Expected Result

The State change should be saved successfully when the State is changed directly through the Incident form.

The onCellEdit Client Script should not block the update because it only prevents State changes made through list editing.

Other configured behaviors should continue to work as expected:

- Assigned To follows the configured validation rules.
- Urgency follows the High Impact UI Policy and Client Script behavior.
- State can be changed through the Incident form.

## Actual Result

The test was successfully completed.

The State field was changed directly from the Incident form and the Incident was successfully updated.

The new State value was saved successfully.

The existing UI Policy and Client Script behavior for other fields continued to function as configured.

## Result

**PASS — Activity 5 completed successfully.**

## Evidence

The screenshot in this folder shows the Incident form after changing the State and successfully updating the record.
