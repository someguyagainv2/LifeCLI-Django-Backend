# LifeCLI-Django-Backend
This is the backend for a game I created for fun there's a lot of flaws however this will be improved over time when I get more in to development of stuff such as handling of SQLI techniques and more.

<h1>Table Content</h1>
initialization
<h2><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/auth">/auth endpoint</a></h2>
<ul>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/auth#login">/login</a></li>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/blob/main/auth/readme.md#create">/create</a></li>
</ul>

<hr>

<h2><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/commands">/commands</a></h2>
<ul>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/commands#beg">/beg</a></li>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/commands#search">/search</a></li>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/commands#fish">/fish</a></li>
    <li>/sell</li>
    <li>/inventory</li>
    <li>/rob</li>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/commands#pickpocket">/pickpocket</a></li>
    <li>/getbalance</li>
    <li>/bank</li>
</ul>

<hr>

<h2><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/phone">/phone</a></h2>
<ul>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/phone#backgroundlookup">/backgroundlookup</a></li>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/phone#createbank">/createbank</a></li>
</ul>

<hr>

<h2><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/store">/store</a></h2>

<ul>
    <li>/buy</li>
    <li>/items</li>
</ul>


<hr>

<h2><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/bank">/bank</a></h2>

<ul>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/bank#deposit">/deposit</a></li>
    <li><a href="https://github.com/someguyagainv2/LifeCLI-Django-Backend/tree/main/bank#withdraw">/withdraw</li>
</ul>

<h1>Status Codes</h1>
True: Successful operation of the command
False: An error occured will be returned in the response

<h1>Auth Endpoint</h1>

BaseURL Example
```http://127.0.0.1:8000/auth```
The auth endpoint handles authentication and can be used to return session IDs, these __sessionIDs__ are crucial for informing the other commands who the person is and checking if it matches up for all of the commands, phone and store endpoint this will rely on a <b>sessionID</b> <u><a href="https://developer.mozilla.org/en-US/docs/Glossary/Request_header">header</a></u>

<h1>Commands Endpoint</h1>

BaseURL Example
```http://127.0.0.1:8000/commands```
The commands endpoint, handles main commands behind the user. The commands are related to user specifically so a sessionID will need to be passed for all commands for a euccessful result. <b>sessionID</b> <u><a href="https://developer.mozilla.org/en-US/docs/Glossary/Request_header">header</a></u>




