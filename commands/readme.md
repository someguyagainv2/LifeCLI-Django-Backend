
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
- SessionID Authorization is incorrect you can get this via /auth/login
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


<h3>/search</h3>

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
- SessionID Authorization is incorrect you can get this via /auth/login
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
response = requests.post("http://127.0.0.1:8000/commands/search", headers={"SessionID": "SessionID"})
print(response.text)
~~~

<hr>


<h3>/pickpocket</h3>

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
- SessionID Authorization is incorrect you can get this via /auth/login
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
response = requests.post("http://127.0.0.1:8000/commands/pickpocket", headers={"SessionID": "SessionID"})
print(response.text)
~~~

<hr>

<h3>/fish</h3>

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
- You do not have fishing rod
- SessionID Authorization is incorrect you can get this via /auth/login
- Item broke had no durability.
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
response = requests.post("http://127.0.0.1:8000/commands/fish", headers={"SessionID": "SessionID"})
print(response.text)
~~~

<h3>/sell</h3>

<table>
    <tr>
        <th>Method</th>
        <th>Headers</th>
        <th>JSON Body</th>
    </tr>
    <tr>
        <td>POST</td>
        <td>SessionID</td>
        <td>ItemName</td>
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
- You do not own this item.
- SessionID Authorization is incorrect you can get this via /auth/login.
- Item does not exist.
~~~

<hr>
<h3>Successful Request Response</h3>

~~~
- Status: True
- Response: Successfully sold for X coins
~~~

<hr>

<h3>Python Code Example</h3>

~~~
import requests
response = requests.post("http://127.0.0.1:8000/commands/sell", headers={"SessionID": "SessionID"}, json={"ItemName": "Item"})
print(response.text)
~~~
<hr>

<h3>/getbalance</h3>

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
- SessionID Authorization is incorrect you can get this via /auth/login
~~~

<hr>
<h3>Successful Request Response</h3>

~~~
- Status: True
- Response: X Cash
~~~

<hr>

<h3>Python Code Example</h3>

~~~
import requests
response = requests.post("http://127.0.0.1:8000/commands/getbalance", headers={"SessionID": "SessionID"})
print(response.text)
~~~
<hr>

<h3>/bank</h3>

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
- SessionID Authorization is incorrect you can get this via /auth/login
~~~

<hr>
<h3>Successful Request Response</h3>

~~~
- Status: True
- Response: X Bank
~~~

<hr>

<h3>Python Code Example</h3>

~~~
import requests
response = requests.post("http://127.0.0.1:8000/commands/bank", headers={"SessionID": "SessionID"})
print(response.text)
~~~
