## Examples

Examples of conditions are:

<table style="WIDTH: 100%">

<tbody>

<tr>

<th>Textual</th>

<th>Logical</th>

</tr>

<tr>

<td>b The customer has a credit cardb </td>

<td>Customer.Credit Card has value</td>

</tr>

<tr>

<td>b The job application is being processedb </td>

<td>Job Application.Status = In Process</td>

</tr>

</tbody>

</table>

In the first example, the condition is evaluated as b trueb  if the Customer has a credit card, i.e. it is evaluated based on the existence of an object (Credit Card). In the second example, the condition is evaluated as b trueb  if the state of the Job Application (the object) is Active, i.e. it is evaluated based on the state of the object.

Examples of conditions on the relationships between objects are:

<table style="WIDTH: 100%">

<tbody>

<tr>

<th>Textual</th>

<th>Logical</th>

</tr>

<tr>

<td>b The person has a submitted timesheetb </td>

<td>Person.Timesheet exists WHERE Timesheet.Status = Submitted</td>

</tr>

<tr>

<td>b The customer has no accepted contracts"</td>

<td>Customer.Contract not exists WHERE Contract.Accepted = True</td>

</tr>

</tbody>

</table>

These examples are evaluated based on relationships between different objects, and the state or existence of these relationships.

Conditions can be combined, i.e. one might define a logical statement about the state of an object and the relationships to other objects at once. For example:

<table style="WIDTH: 100%">

<tbody>

<tr>

<th>Textual</th>

<th>Logical</th>

</tr>

<tr>

<td>b The person is active, and has an active assignment"</td>

<td>Person.State = Active AND Person.Assignment exists WHERE Assignment.State = Active</td>

</tr>

</tbody>

</table>

This example combines 2 conditions (b The person is activeb  and b The person has an active assignmentb ) into one, separated by the logical b ANDb  operator, meaning that both conditions has to be fulfilled. These two conditions might also be separated by the logical b ORb  operation, meaning that statement is true if the person is active, or if the person has an active assignment, or both.