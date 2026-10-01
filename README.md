# Implement Client Script and UI Policy (Incident)


Project Overview

This project demonstrates how to implement UI Policies and different types of Client Scripts on the Incident table in ServiceNow.

The configuration includes:

- UI Policy
- UI Policy Action
- onChange Client Script
- onSubmit Client Script
- onCellEdit Client Script
- Testing and validation

---

Milestone 1: Create UI Policy on Incident

Objective

Create a UI Policy on the Incident table to dynamically control form fields based on specific conditions.

Steps

1. Log in to the ServiceNow instance.
2. Navigate to All → System UI → UI Policies.
3. Click New.
4. Select Incident as the table.
5. Enter a suitable Short description.
6. Define the required condition.
7. Enable On load if the policy should execute when the form loads.
8. Click Submit.

Expected Result

The UI Policy is created successfully and is ready to control the required Incident form fields.

---

Milestone 2: Create UI Policy Action – Urgency

Objective

Create a UI Policy Action to control the Urgency field on the Incident form.

Steps

1. Open the UI Policy created in Milestone 1.
2. Navigate to the UI Policy Actions section.
3. Click New.
4. Select Urgency as the field.
5. Configure the required field behavior, such as:
   - Mandatory
   - Visible
   - Read-only
6. Save the UI Policy Action.
7. Return to the Incident form and verify the behavior.

Expected Result

The Urgency field changes its behavior according to the configured UI Policy condition.

---

Milestone 3: Create onChange Client Script

Objective

Create an onChange Client Script that executes whenever the value of a selected Incident field changes.

Steps

1. Navigate to All → System Definition → Client Scripts.
2. Click New.
3. Select Incident as the table.
4. Select onChange as the Script type.
5. Select the field that should trigger the script.
6. Add the required JavaScript logic.
7. Save the Client Script.
8. Open an Incident record and change the selected field.

Expected Result

The Client Script executes automatically when the selected field value changes.

---

Milestone 4: Create onSubmit Client Script – Save Validation

Objective

Create an onSubmit Client Script to validate Incident information before the record is saved.

Steps

1. Navigate to System Definition → Client Scripts.
2. Click New.
3. Select Incident as the table.
4. Select onSubmit as the Script type.
5. Add the required validation logic.
6. Configure the script to return "true" when validation succeeds.
7. Return "false" when the validation condition is not satisfied.
8. Save the Client Script.
9. Open an Incident and attempt to save it with invalid information.

Expected Result

The Incident record is saved only when the required validation conditions are satisfied.

---

Milestone 5: Create onCellEdit Client Script

Objective

Create an onCellEdit Client Script to validate or control changes made directly from a list view.

Steps

1. Navigate to System Definition → Client Scripts.
2. Click New.
3. Select Incident as the table.
4. Select onCellEdit as the Script type.
5. Add the required JavaScript validation.
6. Configure the script to allow or prevent the list-field modification.
7. Save the Client Script.
8. Navigate to the Incident list.
9. Edit the configured field directly from the list.

Expected Result

The onCellEdit Client Script executes when the selected Incident field is modified directly from the list view.

---

Milestone 6: Testing the Configuration

Objective

Verify that the UI Policy and Client Scripts work correctly.

Testing Steps

UI Policy Testing

1. Open an Incident record.
2. Enter different values that satisfy or do not satisfy the UI Policy condition.
3. Verify the behavior of the Urgency field.
4. Confirm the field's visibility, mandatory status, or read-only status.

onChange Testing

1. Change the configured field.
2. Verify that the Client Script executes.
3. Confirm that the expected form behavior occurs.

onSubmit Testing

1. Enter valid Incident information.
2. Save the record.
3. Verify that the record is saved successfully.
4. Enter invalid information and try saving again.
5. Verify that the validation prevents the record from being saved when required.

onCellEdit Testing

1. Open the Incident list.
2. Edit the configured field directly from the list.
3. Verify that the Client Script executes.
4. Confirm that valid changes are accepted and invalid changes are handled according to the script.

Expected Result

All configured UI Policies and Client Scripts work as expected without errors.

---

Conclusion

The Implement Client Script and UI Policy (Incident) project demonstrates how ServiceNow can be customized using UI Policies and Client Scripts.

The project successfully covers:

- Creating a UI Policy on the Incident table
- Configuring a UI Policy Action for Urgency
- Implementing an onChange Client Script
- Implementing an onSubmit Client Script for save validation
- Implementing an onCellEdit Client Script
- Testing and validating the complete configuration

These configurations improve the dynamic behavior, validation, and user experience of the ServiceNow Incident form and list views.
