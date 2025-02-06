
<h3>/beg</h3>

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
- On cooldown
~~~

<hr>
<h3>Successful Request Response</h3>

~~~
- Status: True
- Response: X Message Random
~~~

<hr>

<h3>Python Code Example</h3>

~~~
import requests
response = requests.post("http://127.0.0.1:8000/commands/beg", headers={"SessionID": "SessionID"})
print(response.text)
~~~

<hr>
