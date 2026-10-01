# Activity 4 — Test List Edit Blocking

## Objective

Verify that users cannot change the Incident State directly through list editing.

## Test Procedure

1. Navigate to **Incident → All**.
2. Open the Incident list.
3. Select an Incident record.
4. Double-click the **State** field to attempt a direct list edit.
5. Attempt to change the State value.
6. Observe the Client Script behavior.

## Expected Result

The onCellEdit Client Script should:

- Display an alert message.
- Prevent the State value from being changed.
- Keep the original State value unchanged.

The expected alert message is:

> State cannot be updated using list editing. Please open the Incident.

## Actual Result

The test was successfully completed.

When an attempt was made to edit the State field directly from the Incident list:

- The warning alert was displayed.
- The list edit operation was blocked.
- The State value remained unchanged.

This confirms that the **onCellEdit Client Script** is working correctly.

## Result

**PASS — Activity 4 completed successfully.**

## Evidence

The screenshot in this folder provides evidence of the list-edit blocking behavior and the displayed warning message.
