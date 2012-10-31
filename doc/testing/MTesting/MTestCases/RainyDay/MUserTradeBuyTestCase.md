## MUserTradeBuyTestCase

### Test Case Description
* Test Case for when a User wants to buy stocks.
* User enters their desired quantity of specified stock.
* System responds with either an error message (unsuccessful) or confirmation (successful).

### Pre-Requisites
* User is verified at log in.

###Rainy Day

<table>
	<tr>
		<th>Inputs</th>
		<th>System Action</th>
		<th>Expected Output</th>
	</tr>
	<tr>
		<td>User enters desired quantity greater than avaliable stock</td>
		<td>System sends error message</td>
		<td>"Quantity desired is un-available -> "user specified amount" "</td>
	</tr>
	<tr>
		<td>User enters ""</td>
		<td>System sends error message</td>
		<td>"Invalid Quantity -> "" must be greater than 0"</td>
	</tr>
	<tr>
		<td>User enters desired quantity greater than their acount balance</td>
		<td>System sends error message</td>
		<td>"Insufficient Funds -> "Account Balance is not equal to needed amount (quantity * stock price)" "</td>
	</tr>
	<tr>
		<td>User enters "-5"</td>
		<td>System sends error message</td>
		<td>"Invalid Quantity -> "-5" must be greater than 0"</td>
	</tr>
	<tr>
		<td>User enters "#$%#"</td>
		<td>System sends error message</td>
		<td>"Invalid Quantity -> "#$%#" must be greater than 0"</td>
	</tr>
</table>
