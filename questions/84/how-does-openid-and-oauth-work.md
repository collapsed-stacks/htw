## How does OpenID and OAuth work?

- posted by: [DTing](https://stackexchange.com/users/-1/62-dting) on 2011-04-18
- tagged: `internet`, `internet-security`
- score: 7

How are one-click login systems like openID and OAuth able to log you in based on being logged into another service?


## Answer 92

- posted by: [StasM](https://stackexchange.com/users/-1/19-stasm) on 2011-04-18
- score: 9

<p><a href="http://en.wikipedia.org/wiki/OpenID" rel="nofollow">OpenID</a> allows you to delegate verification of your identity to some other site. This works as follows:</p>

<ol>
<li>You log in to site A (identity provider)</li>
<li>You go to site B (identity consumer). It asks you for your identity. </li>
<li>You say "ask site A via OpenID".</li>
<li>Site B redirects the request to site A. Since you are already logged in to site A in the browser, site A knows who you are, so it can return to site B with response "this guy is user@siteA".</li>
<li>Site B registers you as "user@siteA".</li>
</ol>

<p>Note that B relies on A to provide true info - i.e., if A lies about the user, B has no way to know it, so you should only accept OAuth providers that you trust if you rely on their data. However, if you just use it as unique name, it's OK to accept any OpenID provider.</p>

<p><a href="http://en.wikipedia.org/wiki/Oauth" rel="nofollow">OAuth</a> is a way to give people (or sites) permissions on certain site without giving them full access and revealing passwords, etc. - e.g., allowing a printing site to access particular image in your photo hosting without giving out your username and password. It works this way:</p>

<ol>
<li>You ask consumer site C to print your photo from provider P.</li>
<li>Site C calls special URL on P and gets a token (random string) called "request token" (RT). </li>
<li>Site C redirects browser request to specific resource on P and uses token RT to cryptographically sign it, so P knows that the request comes from C since it issued RT to C. </li>
<li>Site P displays login form to the user and makes the user identify himself. </li>
<li>Once user is logged in, the site asks "do you approve allowing site C to access this resource"?</li>
<li>If you approve, P generates "authorization token" AT and redirects back to specified URL at C with this token.</li>
<li>C saves the token AT and now can use it to access the specified resource without the user needing to log in again or to give it any access details.</li>
</ol>

<p>Note that the user never gave any details to site C and only asked it to access the specific resource on the site - so if C wanted to access something else it would be denied since the token AT tells site P that it has access for specific resource (unless P issued token that allows access to all - it's up to P to define permissions for each token). </p>

<p>Also the OAuth protocol makes C use its own unique key and generate unique requests with timestamps, so if somebody listened to the request it could not replay it again since P would recognize that it already saw this unique request or because the timestamp is too old, and if someone wanted to fake request from C it wouldn't be able to since it doesn't have C's unique key. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
