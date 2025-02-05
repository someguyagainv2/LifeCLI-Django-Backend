
<h3>/backgroundlookup</h3>

<table>
    <tr>
        <th>payload (json) </th>
        <th>Method</th>
        <th>Headers</th>
    </tr>
    <tr>
        <td>Amount</td>
        <td>POST</td>
        <td>SessionID</td>
    </tr>
</table>

<hr>
<b>Response</b>

JSON Body Response
<table>
    <tr>
        <th>Response JSON Body</th>
    </tr>
    <tr>
        <td>Status</td>
    </tr>
    <tr>
        <td>Response</td>
    </tr>
</table>

<h3>Errors</h3>

~~~
- No bank account
- You don't have that much coins to deposit.
~~~

<hr>
<h3>Successful Request Response</h3>

~~~
- Status: True
- Successfully deposited X coins
~~~

<hr>

<h3>Python Code Example</h3>

~~~
import requests
response = requests.post("http://127.0.0.1:8000/bank/deposit", json={"Amount": 1000}, headers={"SessionID": "SessionID"})
print(response.text)
~~~

<hr>

<h3>/createbank</h3>

<table>
    <tr>
        <th>Method</th>
        <th>Headers</th>
    </tr>
    <tr>
        <td>POST</td>
        <td>SessionID</td>
    </tr>
</table>

<hr>
<b>Response</b>

JSON Body Response
<table>
    <tr>
        <th>Response JSON Body</th>
    </tr>
    <tr>
        <td>Status</td>
    </tr>
    <tr>
        <td>Response</td>
    </tr>
</table>

<h3>Errors</h3>

~~~
- You need a birth certificate as validation to create bank account.
- You need a basic smartphone or advanced smartphone to run this command.
~~~

<hr>
<h3>Successful Request Response</h3>

~~~
- Status: True
- Bank account created.
~~~

<hr>

<h3>Python Code Example</h3>

~~~
import requests
response = requests.post("http://127.0.0.1:8000/phone/createbank", headers={"SessionID": "SessionID"})
print(response.text)
~~~




