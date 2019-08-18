# Adobe I/O CNA Core IMS Library API Documentation

## Modules

<dl>
<dt><a href="#module_@adobe/aio-cna-core-ims">@adobe/aio-cna-core-ims</a></dt>
<dd><p>The <code>@adobe/aio-cna-core-ims</code> module offers three kinds of elements:</p>
<ol>
<li>Managing configuration contexts for token creation and use</li>
<li>Creating and invalidating tokens</li>
<li>Providing low level access to IMS API</li>
</ol>
</dd>
</dl>

## Classes

<dl>
<dt><a href="#Ims">Ims</a></dt>
<dd></dd>
</dl>

## Constants

<dl>
<dt><a href="#context">context</a></dt>
<dd><p>The <code>context</code> object manages the IMS configuration contexts on behalf of
the Adobe I/O CNA Core IMS Library.</p>
</dd>
<dt><a href="#ACCESS_TOKEN">ACCESS_TOKEN</a></dt>
<dd><p>The constant string <code>access_token</code>.</p>
</dd>
<dt><a href="#REFRESH_TOKEN">REFRESH_TOKEN</a></dt>
<dd><p>The constant string <code>refresh_token</code>.</p>
</dd>
<dt><a href="#AUTHORIZATION_CODE">AUTHORIZATION_CODE</a></dt>
<dd><p>The constant string <code>authorization_code</code>.</p>
</dd>
<dt><a href="#CLIENT_ID">CLIENT_ID</a></dt>
<dd><p>The constant string <code>client_id</code>.</p>
</dd>
<dt><a href="#CLIENT_SECRET">CLIENT_SECRET</a></dt>
<dd><p>The constant string <code>client_secret</code>.</p>
</dd>
<dt><a href="#SCOPE">SCOPE</a></dt>
<dd><p>The constant string <code>scope</code>.</p>
</dd>
</dl>

## Functions

<dl>
<dt><a href="#getTokenData">getTokenData(token)</a> ⇒ <code>object</code></dt>
<dd><p>Returns the decoded token value as JavaScript object.</p>
</dd>
</dl>

<a name="module_@adobe/aio-cna-core-ims"></a>

## @adobe/aio-cna-core-ims
The `@adobe/aio-cna-core-ims` module offers three kinds of elements:

1. Managing configuration contexts for token creation and use
2. Creating and invalidating tokens
3. Providing low level access to IMS API


* [@adobe/aio-cna-core-ims](#module_@adobe/aio-cna-core-ims)
    * [.getTokenData](#module_@adobe/aio-cna-core-ims.getTokenData)
    * [.Ims](#module_@adobe/aio-cna-core-ims.Ims)
    * [.ACCESS_TOKEN](#module_@adobe/aio-cna-core-ims.ACCESS_TOKEN)
    * [.REFRESH_TOKEN](#module_@adobe/aio-cna-core-ims.REFRESH_TOKEN)
    * [.AUTHORIZATION_CODE](#module_@adobe/aio-cna-core-ims.AUTHORIZATION_CODE)
    * [.CLIENT_ID](#module_@adobe/aio-cna-core-ims.CLIENT_ID)
    * [.CLIENT_SECRET](#module_@adobe/aio-cna-core-ims.CLIENT_SECRET)
    * [.SCOPE](#module_@adobe/aio-cna-core-ims.SCOPE)
    * [.context](#module_@adobe/aio-cna-core-ims.context)
    * [.getToken(contextName)](#module_@adobe/aio-cna-core-ims.getToken) ⇒ <code>Promise</code>
    * [.invalidateToken(contextName, force)](#module_@adobe/aio-cna-core-ims.invalidateToken)

<a name="module_@adobe/aio-cna-core-ims.getTokenData"></a>

### @adobe/aio-cna-core-ims.getTokenData
**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: (#getTokenData)  
<a name="module_@adobe/aio-cna-core-ims.Ims"></a>

### @adobe/aio-cna-core-ims.Ims
**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: (#Ims)  
<a name="module_@adobe/aio-cna-core-ims.ACCESS_TOKEN"></a>

### @adobe/aio-cna-core-ims.ACCESS\_TOKEN
**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: (#ACCESS_TOKEN)  
<a name="module_@adobe/aio-cna-core-ims.REFRESH_TOKEN"></a>

### @adobe/aio-cna-core-ims.REFRESH\_TOKEN
**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: (#REFRESH_TOKEN)  
<a name="module_@adobe/aio-cna-core-ims.AUTHORIZATION_CODE"></a>

### @adobe/aio-cna-core-ims.AUTHORIZATION\_CODE
**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: (#AUTHORIZATION_CODE)  
<a name="module_@adobe/aio-cna-core-ims.CLIENT_ID"></a>

### @adobe/aio-cna-core-ims.CLIENT\_ID
**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: (#CLIENT_ID)  
<a name="module_@adobe/aio-cna-core-ims.CLIENT_SECRET"></a>

### @adobe/aio-cna-core-ims.CLIENT\_SECRET
**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: (#CLIENT_SECRET)  
<a name="module_@adobe/aio-cna-core-ims.SCOPE"></a>

### @adobe/aio-cna-core-ims.SCOPE
**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: (#SCOPE)  
<a name="module_@adobe/aio-cna-core-ims.context"></a>

### @adobe/aio-cna-core-ims.context
The `context` object manages the IMS configuration contexts on behalf of
the Adobe I/O CNA Core IMS Library.

**Kind**: static property of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**See**: The [`context`](#context) object  
<a name="module_@adobe/aio-cna-core-ims.getToken"></a>

### @adobe/aio-cna-core-ims.getToken(contextName) ⇒ <code>Promise</code>
Returns an access token for the given context name.

**Kind**: static method of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  
**Returns**: <code>Promise</code> - Resolving to an access token (string)  

| Param | Type | Description |
| --- | --- | --- |
| contextName | <code>string</code> | The name of the IMS context for which to              return the access token. If this is empty, the token(s) of              the current IMS context are invalidated. |

<a name="module_@adobe/aio-cna-core-ims.invalidateToken"></a>

### @adobe/aio-cna-core-ims.invalidateToken(contextName, force)
Invalidates the access and optionally refresh of an IMS context.
The name of the IMS context is given as its first parameter and defaults
to the current context if missing or empty. The force parameter indicates
whether only the access token is invalidated (force=false) or the refresh
token (if existing) is also invalidated (force=true). If the refresh token
exists and is validated, all access tokens which have been created with
this refresh token will automatically become invalid as well.

**Kind**: static method of [<code>@adobe/aio-cna-core-ims</code>](#module_@adobe/aio-cna-core-ims)  

| Param | Type | Description |
| --- | --- | --- |
| contextName | <code>string</code> | The name of the IMS context for which to              invalidate the token(s). If this is empty, the token(s) of              the current IMS context are invalidated. |
| force | <code>boolean</code> | Whether to invalidate just the access token or              to also invalidate the refresh token. |

<a name="Ims"></a>

## Ims
**Kind**: global class  

* [Ims](#Ims)
    * [new Ims(env)](#new_Ims_new)
    * _instance_
        * [.getApiUrl(api)](#Ims+getApiUrl) ⇒ <code>string</code>
        * [.getSusiUrl(clientId, scopes, callbackUrl, state)](#Ims+getSusiUrl) ⇒
        * [.get(api, token, parameters)](#Ims+get) ⇒
        * [.post(api, token, parameters)](#Ims+post) ⇒
        * [.getAccessToken(authCode, clientId, clientSecret, scopes)](#Ims+getAccessToken) ⇒
        * [.exchangeJwtToken(clientId, clientSecret, signedJwtToken)](#Ims+exchangeJwtToken)
        * [.invalidateToken(token, clientId, clientSecret)](#Ims+invalidateToken)
        * [.toTokenResult(token)](#Ims+toTokenResult) ⇒
    * _static_
        * [.fromToken(token)](#Ims.fromToken) ⇒

<a name="new_Ims_new"></a>

### new Ims(env)
Creats a new IMS connector instance for the stage or prod environment


| Param | Type | Description |
| --- | --- | --- |
| env | <code>string</code> | The name of the environment. `prod` and `stage`      are the only values supported. `prod` is default and any value      other than `prod` or `stage` stage is assumed to be the default      value of `prod`. |

<a name="Ims+getApiUrl"></a>

### ims.getApiUrl(api) ⇒ <code>string</code>
Returns the absolute URL to call the indicated API.
The API is expected to be the API absolute path, such as `/ims/profile`.
To form the absolute URL, the scheme (`https`) and fully qualified
domain of the IMS host for this instance's environment is prepended
to the path.

**Kind**: instance method of [<code>Ims</code>](#Ims)  
**Returns**: <code>string</code> - The absolute URI for the IMS API  

| Param | Type | Description |
| --- | --- | --- |
| api | <code>string</code> | The API (path) for which to return the URL |

<a name="Ims+getSusiUrl"></a>

### ims.getSusiUrl(clientId, scopes, callbackUrl, state) ⇒
Returns the URL for the environment of this instance which allows
for OAuth2 based three-legged authentication with a browser for
an end user.

**Kind**: instance method of [<code>Ims</code>](#Ims)  
**Returns**: the OAuth2 login URL  

| Param | Type | Description |
| --- | --- | --- |
| clientId | <code>string</code> | The Client ID |
| scopes | <code>string</code> | The list of scopes to request as a blank separated list |
| callbackUrl | <code>string</code> | The callback URL after the user signed in |
| state | <code>string</code> | Any state value which is passed back from sign in |

<a name="Ims+get"></a>

### ims.get(api, token, parameters) ⇒
Send a `GET` request to an IMS API with the access token sending
the `parameters` as request URL parameters.

**Kind**: instance method of [<code>Ims</code>](#Ims)  
**Returns**: a promise resolving to the result of the request  

| Param | Type | Description |
| --- | --- | --- |
| api | <code>string</code> | The IMS API to `GET` from, e.g. `/ims/profile/v1` |
| token | <code>string</code> | The IMS access token to call the API |
| parameters | <code>Map</code> | A map of request parameters |

<a name="Ims+post"></a>

### ims.post(api, token, parameters) ⇒
Send a `POST` request to an IMS API with the access token sending
the `parameters` as form data.

**Kind**: instance method of [<code>Ims</code>](#Ims)  
**Returns**: a promise resolving to the result of the request  

| Param | Type | Description |
| --- | --- | --- |
| api | <code>string</code> | The IMS API to `POST` to, e.g. `/ims/profile/v1` |
| token | <code>string</code> | The IMS access token to call the API |
| parameters | <code>Map</code> | A map of request parameters |

<a name="Ims+getAccessToken"></a>

### ims.getAccessToken(authCode, clientId, clientSecret, scopes) ⇒
Request the access token for the given client providing the access
grant in the `authCode`.
The promise resolve to the token result JavaScript object as follows:

```js
{
  access_token: {
    token: "eyJ4NXUiOi...6ZodTesbag",
    expiry: 1566242851048
  },
  refresh_token: {
    token: "eyJ4NXUiOi...YbT1_szWZA",
    expiry: 1567366051050
  },
  payload: {
     ...full api response...
  }
}
```

**Kind**: instance method of [<code>Ims</code>](#Ims)  
**Returns**: a promise resolving to a tokens object as described in the
     [toTokenResult](toTokenResult) or rejects to an error message.  

| Param | Type | Description |
| --- | --- | --- |
| authCode | <code>string</code> | The authorization code received from the OAuth2      sign in page or by some other means. This may also be a refresh      token which may be traded for a new access token. |
| clientId | <code>string</code> | The Client ID |
| clientSecret | <code>string</code> | The Client Secrete proving client ID ownership |
| scopes | <code>string</code> | The list of scopes to request as a blank separated list |

<a name="Ims+exchangeJwtToken"></a>

### ims.exchangeJwtToken(clientId, clientSecret, signedJwtToken)
Asks for the signed JWT token to be exchanged for a valid access
token as well as a refresh token.
The promise resolve to the token result JavaScript object as follows:

```js
{
  access_token: {
    token: "eyJ4NXUiOi...6ZodTesbag",
    expiry: 1566242851048
  },
  payload: {
     ...full api response...
  }
}
```

Note that there is no `refresh_token` in a JWT tokan exchange.

**Kind**: instance method of [<code>Ims</code>](#Ims)  

| Param | Type | Description |
| --- | --- | --- |
| clientId | <code>string</code> | The client ID of the owning application |
| clientSecret | <code>string</code> | The client's secret |
| signedJwtToken | <code>string</code> | The properly signed JWT token for the JWT token exchange |

<a name="Ims+invalidateToken"></a>

### ims.invalidateToken(token, clientId, clientSecret)
Invalidates the given token. If the token is a refresh token, all the
access tokens created with that refresh token will also be invalidated
at the same time.

**Kind**: instance method of [<code>Ims</code>](#Ims)  

| Param | Type |
| --- | --- |
| token | <code>string</code> | 
| clientId | <code>string</code> | 
| clientSecret | <code>string</code> | 

<a name="Ims+toTokenResult"></a>

### ims.toTokenResult(token) ⇒
Converts the access token to a token result object as follows:

```js
{
  access_token: {
    token: "eyJ4NXUiOi...6ZodTesbag",
    expiry: 1566242851048
  }
}
```

The `expiry` property is the expiry time of the token in milliseconds
since the epoch.

**Kind**: instance method of [<code>Ims</code>](#Ims)  
**Returns**: a `Promise` resolving to an object as described.  

| Param | Type | Description |
| --- | --- | --- |
| token | <code>string</code> | The access token to wrap into a token result |

<a name="Ims.fromToken"></a>

### Ims.fromToken(token) ⇒
Creates an instance of the `Ims` class deriving the instance's
environment from the `as` claim in the provided access token.

**Kind**: static method of [<code>Ims</code>](#Ims)  
**Returns**: A `Promise` resolving to the `Ims` instance.  

| Param | Type | Description |
| --- | --- | --- |
| token | <code>string</code> | The access token from which to extract the      environment to setup the `Ims` instancee. |

<a name="context"></a>

## context
The `context` object manages the IMS configuration contexts on behalf of
the Adobe I/O CNA Core IMS Library.

**Kind**: global constant  

* [context](#context)
    * [.current](#context.current)
    * [.plugins](#context.plugins)
    * [.setCurrent(contextName, local)](#context.setCurrent)
    * [.keys()](#context.keys) ⇒ <code>Array.&lt;string&gt;</code>
    * [.get(contextName)](#context.get) ⇒ <code>object</code>
    * [.set(contextName, contextData, local)](#context.set)

<a name="context.current"></a>

### context.current
The current context name.
When assigning a value, the name is persisted in the local configuration.
To persist the new current context name in global configuration call the
`setCurrent(contextName, local)` method with `local=false`.

**Kind**: static property of [<code>context</code>](#context)  
<a name="context.plugins"></a>

### context.plugins
The list of additional IMS login plugins to consider.
The JWT and OAuth2 plugins are required by the CNA Core IMS
library and are always installed and used.
This list of plugins is always stored in the global configuration.

**Kind**: static property of [<code>context</code>](#context)  
<a name="context.setCurrent"></a>

### context.setCurrent(contextName, local)
Sets the current context name while explicitly stating whether to
persist in the local or global configuration.

**Kind**: static method of [<code>context</code>](#context)  

| Param | Type | Description |
| --- | --- | --- |
| contextName | <code>string</code> | The name of the context to use as the current context |
| local | <code>boolean</code> | Persist the current name in local (`true`) or      global (`false`, default) configuration |

<a name="context.keys"></a>

### context.keys() ⇒ <code>Array.&lt;string&gt;</code>
Returns the names of the configured IMS contexts as an array of strings.

**Kind**: static method of [<code>context</code>](#context)  
**Returns**: <code>Array.&lt;string&gt;</code> - The names of the currently known configurations.  
<a name="context.get"></a>

### context.get(contextName) ⇒ <code>object</code>
Returns an object representing the named context.
If the contextName parameter is empty or missing, it defaults to the
current context name. The result is an object with two properties:

  - `name`: The actual context name used
  - `data`: The IMS context data

**Kind**: static method of [<code>context</code>](#context)  
**Returns**: <code>object</code> - The configuration object  

| Param | Type | Description |
| --- | --- | --- |
| contextName | <code>string</code> | Name of the context information to return. |

<a name="context.set"></a>

### context.set(contextName, contextData, local)
Updates the named configuration with new configuration data.
If a configuration object for the named context already exists it
is completely replaced with this new configuration.

**Kind**: static method of [<code>context</code>](#context)  

| Param | Type | Description |
| --- | --- | --- |
| contextName | <code>string</code> | Name of the context to update |
| contextData | <code>object</code> | The configuration data to store for the context |
| local | <code>boolean</code> | Persist in local (`true`) or global (`false`,          default) configuration |

<a name="ACCESS_TOKEN"></a>

## ACCESS\_TOKEN
The constant string `access_token`.

**Kind**: global constant  
<a name="REFRESH_TOKEN"></a>

## REFRESH\_TOKEN
The constant string `refresh_token`.

**Kind**: global constant  
<a name="AUTHORIZATION_CODE"></a>

## AUTHORIZATION\_CODE
The constant string `authorization_code`.

**Kind**: global constant  
<a name="CLIENT_ID"></a>

## CLIENT\_ID
The constant string `client_id`.

**Kind**: global constant  
<a name="CLIENT_SECRET"></a>

## CLIENT\_SECRET
The constant string `client_secret`.

**Kind**: global constant  
<a name="SCOPE"></a>

## SCOPE
The constant string `scope`.

**Kind**: global constant  
<a name="getTokenData"></a>

## getTokenData(token) ⇒ <code>object</code>
Returns the decoded token value as JavaScript object.

**Kind**: global function  
**Returns**: <code>object</code> - The decoded token payload data without header and signature  

| Param | Type | Description |
| --- | --- | --- |
| token | <code>string</code> | The token to decode and extract the token value from |
