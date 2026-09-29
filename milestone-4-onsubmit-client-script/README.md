# Milestone 4 — onSubmit Client Script

## Objective

Create an onSubmit Client Script for the Incident table that prevents a High Impact Incident from being saved when the Assigned To field is empty.

## Client Script Configuration

| Configuration | Value |
|---|---|
| Name | Prevent save if Assigned To missing |
| Table | Incident |
| Type | onSubmit |
| Active | True |

## Script Behavior

The Client Script executes when the user attempts to submit or save an Incident record.

The script checks two conditions:

1. Impact is set to `1 - High`
2. Assigned To is empty

If both conditions are true, the script:

- Displays an error message on the Assigned To field.
- Prevents the Incident from being saved by returning `false`.

If the conditions are not met, the script returns `true` and allows the record to be saved.

## Script

```javascript
function onSubmit() {
    if (g_form.getValue('impact') == '1' &&
        g_form.getValue('assigned_to') == '') {

        g_form.showErrorBox(
            'assigned_to',
            'Assigned To is mandatory for High impact incidents.'
        );
        return false;
    }
    return true;
}
