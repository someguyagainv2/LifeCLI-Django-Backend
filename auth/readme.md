<h3>/login</h3>

<table>
    <tr>
        <th>payload (json) </th>
        <th>Method</th>
    </tr>
    <tr>
        <td>username</td>
        <td>POST</td>
    </tr>
    <tr>
        <td>password</td>
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
        <td>sessionID</td>
    </tr>
</table>

<h3>Error Occuring</h3>
JSON Body Response
<table>
    <tr>
        <th>JSON Body</th>
    </tr>
    <tr>
        <td>Status</td>
    </tr>
    <tr>
        <td>Error</td>
    </tr>
</table>

<h3>Successful Request Response</h3>

~~~
{
    "Status": true, 
    "sessionID": ""
}
~~~
<hr>

<h3>Python Code Example</h3>

~~~
import requests
response = requests.post("http://127.0.0.1:8000/auth/login", json={"username": "user", "password": "pass"})
print(response.text)
~~~

<h3>/create</h3>

<table>
    <tr>
        <th>payload (json) </th>
        <th>Method</th>
    </tr>
    <tr>
        <td>username</td>
        <td>POST</td>
    </tr>
    <tr>
        <td>password</td>
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
</table>

<h3>Error Occuring</h3>
JSON Body Response
<table>
    <tr>
        <th>JSON Body</th>
    </tr>
    <tr>
        <td>Status</td>
    </tr>
    <tr>
        <td>Error</td>
    </tr>
</table>

<h3>Successful Request Response</h3>

~~~
{
    "Status": true
}
~~~
<hr>

<h3>Python Code Example</h3>

~~~
import requests
response = requests.post("http://127.0.0.1:8000/auth/create", json={"username": "user", "password": "pass"})
print(response.text)
~~~

