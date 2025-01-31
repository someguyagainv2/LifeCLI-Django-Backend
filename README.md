# LifeCLI-Django-Backend
This is the backend for a game I created for fun there's a lot of flaws however this will be improved over time when I get more in to development of stuff such as handling of SQLI techniques and more.

<h1>Table Content</h1>
initialization
<h2>/auth endpoint</h2>
<ul>
    <li>/login</li>
    <li>/create</li>
</ul>

<hr>

<h2>/commands</h2>
<ul>
    <li>/beg</li>
    <li>/search</li>
    <li>/fish</li>
    <li>/sell</li>
    <li>/inventory</li>
    <li>/rob</li>
    <li>/pickpocket</li>
    <li>/getbalance</li>
    <li>/bank</li>
</ul>

<hr>

<h2>/phone</h2>
<ul>
    <li>backgroundlookup</li>
    <li>createbank</li>
</ul>

<hr>

<h2>/store</h2>

<ul>
    <li>/buy</li>
    <li>/items</li>
</ul>


<hr>

<h2>/bank</h2>

<ul>
    <li>/deposit</li>
    <li>/withdraw</li>
</ul>

<h1>Status Codes</h1>
True: Successful operation of the command
False: An error occured will be returned in the response

<h1>auth endpoint</h1>

BaseURL Example
```http://127.0.0.1:8000/auth```
The auth endpoint handles authentication and can be used to return session IDs, these __sessionIDs__ are crucial for informing the other commands who the person is and checking if it matches up for all of the commands, phone and store endpoint this will rely on a <b>sessionID</b> <u><a href="https://developer.mozilla.org/en-US/docs/Glossary/Request_header">header</a></u>

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

<h3>Python Code Example</h3>

<code>
    import requests
    response = requests.post("http://127.0.0.1:8000/auth/login", json={"username": "user", "password": "pass"})
    print(response.text)
</code>
