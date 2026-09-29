# Milestone 5 — onCellEdit Client Script

## Objective

Create an onCellEdit Client Script for the Incident table to prevent users from changing the State field directly through list editing.

## Client Script Configuration

| Configuration | Value |
|---|---|
| Name | Prevent state change via list edit |
| Table | Incident |
| Type | onCellEdit |
| Field name | State |
| Active | True |

## Script Behavior

The Client Script executes when a user attempts to edit the State field directly from an Incident list.

The script displays the following warning:

> State cannot be updated using list editing. Please open the Incident.

The script then uses `callback(false)` to reject the list edit operation and prevent the State value from being changed.

## Script

```javascript
function onCellEdit(sysIDs, table, oldValues, newValue, callback) {

    alert('State cannot be updated using list editing. Please open the Incident.');

    callback(false);
}
