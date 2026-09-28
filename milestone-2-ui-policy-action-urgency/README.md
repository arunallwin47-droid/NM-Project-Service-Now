# Milestone 2 — UI Policy Action: Urgency

## Objective

Extend the existing `High Impact Control` UI Policy by creating a UI Policy Action that controls the Urgency field on the Incident form.

## Existing UI Policy

- **UI Policy:** High Impact Control
- **Table:** Incident
- **Condition:** Impact is 1 - High

## UI Policy Action Configuration

A new UI Policy Action was created under the `High Impact Control` UI Policy.

| Configuration | Value |
|---|---|
| UI Policy | High Impact Control |
| Table | Incident |
| Field name | Urgency |
| Read-only | True |
| Visible | Leave alone |
| Mandatory | Leave alone |
| Clear the field value | Unchecked |

## Behavior

When the Incident Impact is set to `1 - High`, the `High Impact Control` UI Policy is triggered.

The UI Policy Action then makes the **Urgency** field read-only.

The field remains visible on the Incident form, but users cannot modify it while the UI Policy condition is active.

## Implementation Steps

1. Opened the existing `High Impact Control` UI Policy.
2. Navigated to the **UI Policy Actions** related list.
3. Clicked **New** to create a new UI Policy Action.
4. Selected **Urgency** as the field name.
5. Set **Read-only** to `True`.
6. Left **Visible** as `Leave alone`.
7. Left the remaining action settings unchanged.
8. Submitted the UI Policy Action.

## Milestone Status

**Completed — Submitted for Review**

## Evidence

ServiceNow configuration screenshots and implementation evidence are included in this folder.
