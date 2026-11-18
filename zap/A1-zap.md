# ZAP Scanning Report

ZAP by [Checkmarx](https://checkmarx.com/).


## Summary of Alerts

| Risk Level | Number of Alerts |
| --- | --- |
| High | 0 |
| Medium | 3 |
| Low | 7 |
| Informational | 5 |




## Insights

| Level | Reason | Site | Description | Statistic |
| --- | --- | --- | --- | --- |
| Low | Warning |  | ZAP warnings logged - see the zap.log file for details | 10    |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of responses with status code 2xx | 97 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of responses with status code 4xx | 2 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of endpoints with content type application/javascript | 2 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of endpoints with content type image/vnd.microsoft.icon | 2 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of endpoints with content type text/css | 2 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of endpoints with content type text/html | 12 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of endpoints with content type text/javascript | 77 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of endpoints with content type text/plain | 2 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of endpoints with method GET | 100 % |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Count of total endpoints | 40    |
| Info | Informational | https://tarefa-time-organizador.lovable.app | Percentage of slow responses | 97 % |







## Alerts

| Name | Risk Level | Number of Instances |
| --- | --- | --- |
| Content Security Policy (CSP) Header Not Set | Medium | 5 |
| Missing Anti-clickjacking Header | Medium | 4 |
| Sub Resource Integrity Attribute Missing | Medium | 5 |
| Cookie with SameSite Attribute None | Low | 1 |
| Cookie without SameSite Attribute | Low | 3 |
| Cross-Origin-Embedder-Policy Header Missing or Invalid | Low | 1 |
| Cross-Origin-Opener-Policy Header Missing or Invalid | Low | 1 |
| Cross-Origin-Resource-Policy Header Missing or Invalid | Low | Systemic |
| Permissions Policy Header Not Set | Low | Systemic |
| Timestamp Disclosure - Unix | Low | Systemic |
| Loosely Scoped Cookie | Informational | 3 |
| Re-examine Cache-control Directives | Informational | 5 |
| Session Management Response Identified | Informational | 3 |
| Storable and Cacheable Content | Informational | Systemic |
| Storable but Non-Cacheable Content | Informational | 1 |




## Alert Detail



### [ Content Security Policy (CSP) Header Not Set ](https://www.zaproxy.org/docs/alerts/10038/)



##### Medium (High)

### Description

Content Security Policy (CSP) is an added layer of security that helps to detect and mitigate certain types of attacks, including Cross Site Scripting (XSS) and data injection attacks. These attacks are used for everything from data theft to site defacement or distribution of malware. CSP provides a set of standard HTTP headers that allow website owners to declare approved sources of content that browsers should be allowed to load on that page — covered types are JavaScript, CSS, HTML frames, fonts, images and embeddable objects such as Java applets, ActiveX, audio and video files.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/auth
  * Node Name: `https://tarefa-time-organizador.lovable.app/auth`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/auth%3Fmodo=cadastro
  * Node Name: `https://tarefa-time-organizador.lovable.app/auth (modo)`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/esqueci-senha
  * Node Name: `https://tarefa-time-organizador.lovable.app/esqueci-senha`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/sitemap.xml
  * Node Name: `https://tarefa-time-organizador.lovable.app/sitemap.xml`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``


Instances: 5

### Solution

Ensure that your web server, application server, load balancer, etc. is configured to set the Content-Security-Policy header.

### Reference


* [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CSP ](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CSP)
* [ https://cheatsheetseries.owasp.org/cheatsheets/Content_Security_Policy_Cheat_Sheet.html ](https://cheatsheetseries.owasp.org/cheatsheets/Content_Security_Policy_Cheat_Sheet.html)
* [ https://www.w3.org/TR/CSP/ ](https://www.w3.org/TR/CSP/)
* [ https://w3c.github.io/webappsec-csp/ ](https://w3c.github.io/webappsec-csp/)
* [ https://web.dev/articles/csp ](https://web.dev/articles/csp)
* [ https://caniuse.com/#feat=contentsecuritypolicy ](https://caniuse.com/#feat=contentsecuritypolicy)
* [ https://content-security-policy.com/ ](https://content-security-policy.com/)


#### CWE Id: [ 693 ](https://cwe.mitre.org/data/definitions/693.html)


#### WASC Id: 15

#### Source ID: 3

### [ Missing Anti-clickjacking Header ](https://www.zaproxy.org/docs/alerts/10020/)



##### Medium (Medium)

### Description

The response does not protect against 'ClickJacking' attacks. It should include either Content-Security-Policy with 'frame-ancestors' directive or X-Frame-Options.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `x-frame-options`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/auth
  * Node Name: `https://tarefa-time-organizador.lovable.app/auth`
  * Method: `GET`
  * Parameter: `x-frame-options`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/auth%3Fmodo=cadastro
  * Node Name: `https://tarefa-time-organizador.lovable.app/auth (modo)`
  * Method: `GET`
  * Parameter: `x-frame-options`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/esqueci-senha
  * Node Name: `https://tarefa-time-organizador.lovable.app/esqueci-senha`
  * Method: `GET`
  * Parameter: `x-frame-options`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``


Instances: 4

### Solution

Modern Web browsers support the Content-Security-Policy and X-Frame-Options HTTP headers. Ensure one of them is set on all web pages returned by your site/app.
If you expect the page to be framed only by pages on your server (e.g. it's part of a FRAMESET) then you'll want to use SAMEORIGIN, otherwise if you never expect the page to be framed, you should use DENY. Alternatively consider implementing Content Security Policy's "frame-ancestors" directive.

### Reference


* [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/X-Frame-Options ](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/X-Frame-Options)


#### CWE Id: [ 1021 ](https://cwe.mitre.org/data/definitions/1021.html)


#### WASC Id: 15

#### Source ID: 3

### [ Sub Resource Integrity Attribute Missing ](https://www.zaproxy.org/docs/alerts/90003/)



##### Medium (High)

### Description

The integrity attribute is missing on a script or link tag served by an external server. The integrity tag prevents an attacker who have gained access to this server from injecting a malicious content.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700&amp;family=Sora:wght@500;600;700&amp;display=swap" data-precedence="default"/>`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/auth
  * Node Name: `https://tarefa-time-organizador.lovable.app/auth`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700&amp;family=Sora:wght@500;600;700&amp;display=swap" data-precedence="default"/>`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/auth%3Fmodo=cadastro
  * Node Name: `https://tarefa-time-organizador.lovable.app/auth (modo)`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700&amp;family=Sora:wght@500;600;700&amp;display=swap" data-precedence="default"/>`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/esqueci-senha
  * Node Name: `https://tarefa-time-organizador.lovable.app/esqueci-senha`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700&amp;family=Sora:wght@500;600;700&amp;display=swap" data-precedence="default"/>`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/sitemap.xml
  * Node Name: `https://tarefa-time-organizador.lovable.app/sitemap.xml`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700&amp;family=Sora:wght@500;600;700&amp;display=swap" data-precedence="default"/>`
  * Other Info: ``


Instances: 5

### Solution

Provide a valid integrity attribute to the tag.

### Reference


* [ https://developer.mozilla.org/en-US/docs/Web/Security/Defenses/Subresource_Integrity ](https://developer.mozilla.org/en-US/docs/Web/Security/Defenses/Subresource_Integrity)


#### CWE Id: [ 345 ](https://cwe.mitre.org/data/definitions/345.html)


#### WASC Id: 15

#### Source ID: 3

### [ Cookie with SameSite Attribute None ](https://www.zaproxy.org/docs/alerts/10054/)



##### Low (Medium)

### Description

A cookie has been set with its SameSite attribute set to "none", which means that the cookie can be sent as a result of a 'cross-site' request. The SameSite attribute is an effective counter measure to cross-site request forgery, cross-site script inclusion, and timing attacks.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `__cf_bm`
  * Attack: ``
  * Evidence: `set-cookie: __cf_bm`
  * Other Info: ``


Instances: 1

### Solution

Ensure that the SameSite attribute is set to either 'lax' or ideally 'strict' for all cookies.

### Reference


* [ https://datatracker.ietf.org/doc/html/draft-ietf-httpbis-cookie-same-site ](https://datatracker.ietf.org/doc/html/draft-ietf-httpbis-cookie-same-site)


#### CWE Id: [ 1275 ](https://cwe.mitre.org/data/definitions/1275.html)


#### WASC Id: 13

#### Source ID: 3

### [ Cookie without SameSite Attribute ](https://www.zaproxy.org/docs/alerts/10054/)



##### Low (Medium)

### Description

A cookie has been set without the SameSite attribute, which means that the cookie can be sent as a result of a 'cross-site' request. The SameSite attribute is an effective counter measure to cross-site request forgery, cross-site script inclusion, and timing attacks.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `__cf_bm`
  * Attack: ``
  * Evidence: `set-cookie: __cf_bm`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/robots.txt
  * Node Name: `https://tarefa-time-organizador.lovable.app/robots.txt`
  * Method: `GET`
  * Parameter: `__cf_bm`
  * Attack: ``
  * Evidence: `set-cookie: __cf_bm`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/sitemap.xml
  * Node Name: `https://tarefa-time-organizador.lovable.app/sitemap.xml`
  * Method: `GET`
  * Parameter: `__cf_bm`
  * Attack: ``
  * Evidence: `set-cookie: __cf_bm`
  * Other Info: ``


Instances: 3

### Solution

Ensure that the SameSite attribute is set to either 'lax' or ideally 'strict' for all cookies.

### Reference


* [ https://datatracker.ietf.org/doc/html/draft-ietf-httpbis-cookie-same-site ](https://datatracker.ietf.org/doc/html/draft-ietf-httpbis-cookie-same-site)


#### CWE Id: [ 1275 ](https://cwe.mitre.org/data/definitions/1275.html)


#### WASC Id: 13

#### Source ID: 3

### [ Cross-Origin-Embedder-Policy Header Missing or Invalid ](https://www.zaproxy.org/docs/alerts/90004/)



##### Low (Medium)

### Description

Cross-Origin-Embedder-Policy header is a response header that prevents a document from loading any cross-origin resources that don't explicitly grant the document permission (using CORP or CORS).

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `Cross-Origin-Embedder-Policy`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``


Instances: 1

### Solution

Ensure that the application/web server sets the Cross-Origin-Embedder-Policy header appropriately, and that it sets the Cross-Origin-Embedder-Policy header to 'require-corp' for documents.
If possible, ensure that the end user uses a standards-compliant and modern web browser that supports the Cross-Origin-Embedder-Policy header (https://caniuse.com/mdn-http_headers_cross-origin-embedder-policy).

### Reference


* [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Cross-Origin-Embedder-Policy ](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Cross-Origin-Embedder-Policy)


#### CWE Id: [ 693 ](https://cwe.mitre.org/data/definitions/693.html)


#### WASC Id: 14

#### Source ID: 3

### [ Cross-Origin-Opener-Policy Header Missing or Invalid ](https://www.zaproxy.org/docs/alerts/90004/)



##### Low (Medium)

### Description

Cross-Origin-Opener-Policy header is a response header that allows a site to control if others included documents share the same browsing context. Sharing the same browsing context with untrusted documents might lead to data leak.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `Cross-Origin-Opener-Policy`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``


Instances: 1

### Solution

Ensure that the application/web server sets the Cross-Origin-Opener-Policy header appropriately, and that it sets the Cross-Origin-Opener-Policy header to 'same-origin' for documents.
'same-origin-allow-popups' is considered as less secured and should be avoided.
If possible, ensure that the end user uses a standards-compliant and modern web browser that supports the Cross-Origin-Opener-Policy header (https://caniuse.com/mdn-http_headers_cross-origin-opener-policy).

### Reference


* [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Cross-Origin-Opener-Policy ](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Cross-Origin-Opener-Policy)


#### CWE Id: [ 693 ](https://cwe.mitre.org/data/definitions/693.html)


#### WASC Id: 14

#### Source ID: 3

### [ Cross-Origin-Resource-Policy Header Missing or Invalid ](https://www.zaproxy.org/docs/alerts/90004/)



##### Low (Medium)

### Description

Cross-Origin-Resource-Policy header is an opt-in header designed to counter side-channels attacks like Spectre. Resource should be specifically set as shareable amongst different origins.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `Cross-Origin-Resource-Policy`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/__l5e/events.270c78a44fc53e7b.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/__l5e/events.270c78a44fc53e7b.js`
  * Method: `GET`
  * Parameter: `Cross-Origin-Resource-Policy`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/assets/matchContext-Cb-2A7T7.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/assets/matchContext-Cb-2A7T7.js`
  * Method: `GET`
  * Parameter: `Cross-Origin-Resource-Policy`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/robots.txt
  * Node Name: `https://tarefa-time-organizador.lovable.app/robots.txt`
  * Method: `GET`
  * Parameter: `Cross-Origin-Resource-Policy`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/~flock.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/~flock.js`
  * Method: `GET`
  * Parameter: `Cross-Origin-Resource-Policy`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``

Instances: Systemic


### Solution

Ensure that the application/web server sets the Cross-Origin-Resource-Policy header appropriately, and that it sets the Cross-Origin-Resource-Policy header to 'same-origin' for all web pages.
'same-site' is considered as less secured and should be avoided.
If resources must be shared, set the header to 'cross-origin'.
If possible, ensure that the end user uses a standards-compliant and modern web browser that supports the Cross-Origin-Resource-Policy header (https://caniuse.com/mdn-http_headers_cross-origin-resource-policy).

### Reference


* [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Cross-Origin-Embedder-Policy ](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Cross-Origin-Embedder-Policy)


#### CWE Id: [ 693 ](https://cwe.mitre.org/data/definitions/693.html)


#### WASC Id: 14

#### Source ID: 3

### [ Permissions Policy Header Not Set ](https://www.zaproxy.org/docs/alerts/10063/)



##### Low (Medium)

### Description

Permissions Policy Header is an added layer of security that helps to restrict from unauthorized access or usage of browser/client features by web resources. This policy ensures the user privacy by limiting or specifying the features of the browsers can be used by the web resources. Permissions Policy provides a set of standard HTTP headers that allow website owners to limit which features of browsers can be used by the page such as camera, microphone, location, full screen etc.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/__l5e/events.270c78a44fc53e7b.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/__l5e/events.270c78a44fc53e7b.js`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/assets/matchContext-Cb-2A7T7.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/assets/matchContext-Cb-2A7T7.js`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/sitemap.xml
  * Node Name: `https://tarefa-time-organizador.lovable.app/sitemap.xml`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/~flock.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/~flock.js`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: ``

Instances: Systemic


### Solution

Ensure that your web server, application server, load balancer, etc. is configured to set the Permissions-Policy header.

### Reference


* [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Permissions-Policy ](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Permissions-Policy)
* [ https://developer.chrome.com/blog/feature-policy/ ](https://developer.chrome.com/blog/feature-policy/)
* [ https://scotthelme.co.uk/a-new-security-header-feature-policy/ ](https://scotthelme.co.uk/a-new-security-header-feature-policy/)
* [ https://w3c.github.io/webappsec-feature-policy/ ](https://w3c.github.io/webappsec-feature-policy/)
* [ https://www.smashingmagazine.com/2018/12/feature-policy/ ](https://www.smashingmagazine.com/2018/12/feature-policy/)


#### CWE Id: [ 693 ](https://cwe.mitre.org/data/definitions/693.html)


#### WASC Id: 15

#### Source ID: 3

### [ Timestamp Disclosure - Unix ](https://www.zaproxy.org/docs/alerts/10096/)



##### Low (Low)

### Description

A timestamp was disclosed by the application/web server. - Unix

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `set-cookie`
  * Attack: ``
  * Evidence: `1794069880`
  * Other Info: `1794069880, which evaluates to: 2026-11-07 16:44:40.`
* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `x-deployment-id`
  * Attack: ``
  * Evidence: `1794674680`
  * Other Info: `1794674680, which evaluates to: 2026-11-14 16:44:40.`
* URL: https://tarefa-time-organizador.lovable.app/robots.txt
  * Node Name: `https://tarefa-time-organizador.lovable.app/robots.txt`
  * Method: `GET`
  * Parameter: `set-cookie`
  * Attack: ``
  * Evidence: `1794069880`
  * Other Info: `1794069880, which evaluates to: 2026-11-07 16:44:40.`
* URL: https://tarefa-time-organizador.lovable.app/robots.txt
  * Node Name: `https://tarefa-time-organizador.lovable.app/robots.txt`
  * Method: `GET`
  * Parameter: `x-deployment-id`
  * Attack: ``
  * Evidence: `1794674680`
  * Other Info: `1794674680, which evaluates to: 2026-11-14 16:44:40.`
* URL: https://tarefa-time-organizador.lovable.app/sitemap.xml
  * Node Name: `https://tarefa-time-organizador.lovable.app/sitemap.xml`
  * Method: `GET`
  * Parameter: `set-cookie`
  * Attack: ``
  * Evidence: `1794069880`
  * Other Info: `1794069880, which evaluates to: 2026-11-07 16:44:40.`

Instances: Systemic


### Solution

Manually confirm that the timestamp data is not sensitive, and that the data cannot be aggregated to disclose exploitable patterns.

### Reference


* [ https://cwe.mitre.org/data/definitions/200.html ](https://cwe.mitre.org/data/definitions/200.html)


#### CWE Id: [ 497 ](https://cwe.mitre.org/data/definitions/497.html)


#### WASC Id: 13

#### Source ID: 3

### [ Loosely Scoped Cookie ](https://www.zaproxy.org/docs/alerts/90033/)



##### Informational (Low)

### Description

Cookies can be scoped by domain or path. This check is only concerned with domain scope.The domain scope applied to a cookie determines which domains can access it. For example, a cookie can be scoped strictly to a subdomain e.g. www.nottrusted.com, or loosely scoped to a parent domain e.g. nottrusted.com. In the latter case, any subdomain of nottrusted.com can access the cookie. Loosely scoped cookies are common in mega-applications like google.com and live.com. Cookies set from a subdomain like app.foo.bar are transmitted only to that domain by the browser. However, cookies scoped to a parent-level domain may be transmitted to the parent, or any subdomain of the parent.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `Domain=lovable.app`
  * Other Info: `The origin domain used for comparison was:
tarefa-time-organizador.lovable.app
Cookie name: __cf_bm
`
* URL: https://tarefa-time-organizador.lovable.app/robots.txt
  * Node Name: `https://tarefa-time-organizador.lovable.app/robots.txt`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `Domain=lovable.app`
  * Other Info: `The origin domain used for comparison was:
tarefa-time-organizador.lovable.app
Cookie name: __cf_bm
`
* URL: https://tarefa-time-organizador.lovable.app/sitemap.xml
  * Node Name: `https://tarefa-time-organizador.lovable.app/sitemap.xml`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `Domain=lovable.app`
  * Other Info: `The origin domain used for comparison was:
tarefa-time-organizador.lovable.app
Cookie name: __cf_bm
`


Instances: 3

### Solution

Always scope cookies to a FQDN (Fully Qualified Domain Name).

### Reference


* [ https://datatracker.ietf.org/doc/html/rfc6265#section-4.1 ](https://datatracker.ietf.org/doc/html/rfc6265#section-4.1)
* [ https://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/06-Session_Management_Testing/02-Testing_for_Cookies_Attributes.html ](https://owasp.org/www-project-web-security-testing-guide/v41/4-Web_Application_Security_Testing/06-Session_Management_Testing/02-Testing_for_Cookies_Attributes.html)
* [ https://code.google.com/archive/p/browsersec/wikis/Part2.wiki ](https://code.google.com/archive/p/browsersec/wikis/Part2.wiki)


#### CWE Id: [ 565 ](https://cwe.mitre.org/data/definitions/565.html)


#### WASC Id: 15

#### Source ID: 3

### [ Re-examine Cache-control Directives ](https://www.zaproxy.org/docs/alerts/10015/)



##### Informational (Low)

### Description

The cache-control header has not been set properly or is missing, allowing the browser and proxies to cache content. For static assets like css, js, or image files this might be intended, however, the resources should be reviewed to ensure that no sensitive content will be cached.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `cache-control`
  * Attack: ``
  * Evidence: `no-cache, must-revalidate, max-age=0`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/auth
  * Node Name: `https://tarefa-time-organizador.lovable.app/auth`
  * Method: `GET`
  * Parameter: `cache-control`
  * Attack: ``
  * Evidence: `no-cache, must-revalidate, max-age=0`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/auth%3Fmodo=cadastro
  * Node Name: `https://tarefa-time-organizador.lovable.app/auth (modo)`
  * Method: `GET`
  * Parameter: `cache-control`
  * Attack: ``
  * Evidence: `no-cache, must-revalidate, max-age=0`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/esqueci-senha
  * Node Name: `https://tarefa-time-organizador.lovable.app/esqueci-senha`
  * Method: `GET`
  * Parameter: `cache-control`
  * Attack: ``
  * Evidence: `no-cache, must-revalidate, max-age=0`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/robots.txt
  * Node Name: `https://tarefa-time-organizador.lovable.app/robots.txt`
  * Method: `GET`
  * Parameter: `cache-control`
  * Attack: ``
  * Evidence: ``
  * Other Info: ``


Instances: 5

### Solution

For secure content, ensure the cache-control HTTP header is set with "no-cache, no-store, must-revalidate". If an asset should be cached consider setting the directives "public, max-age, immutable".

### Reference


* [ https://cheatsheetseries.owasp.org/cheatsheets/Session_Management_Cheat_Sheet.html#web-content-caching ](https://cheatsheetseries.owasp.org/cheatsheets/Session_Management_Cheat_Sheet.html#web-content-caching)
* [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Cache-Control ](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Cache-Control)
* [ https://grayduck.mn/2021/09/13/cache-control-recommendations/ ](https://grayduck.mn/2021/09/13/cache-control-recommendations/)


#### CWE Id: [ 525 ](https://cwe.mitre.org/data/definitions/525.html)


#### WASC Id: 13

#### Source ID: 3

### [ Session Management Response Identified ](https://www.zaproxy.org/docs/alerts/10112/)



##### Informational (Medium)

### Description

The given response has been identified as containing a session management token. The 'Other Info' field contains a set of header tokens that can be used in the Header Based Session Management Method. If the request is in a context which has a Session Management Method set to "Auto-Detect" then this rule will change the session management to use the tokens identified.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: `__cf_bm`
  * Attack: ``
  * Evidence: `__cf_bm`
  * Other Info: `cookie:__cf_bm`
* URL: https://tarefa-time-organizador.lovable.app/robots.txt
  * Node Name: `https://tarefa-time-organizador.lovable.app/robots.txt`
  * Method: `GET`
  * Parameter: `__cf_bm`
  * Attack: ``
  * Evidence: `__cf_bm`
  * Other Info: `cookie:__cf_bm`
* URL: https://tarefa-time-organizador.lovable.app/sitemap.xml
  * Node Name: `https://tarefa-time-organizador.lovable.app/sitemap.xml`
  * Method: `GET`
  * Parameter: `__cf_bm`
  * Attack: ``
  * Evidence: `__cf_bm`
  * Other Info: `cookie:__cf_bm`


Instances: 3

### Solution

This is an informational alert rather than a vulnerability and so there is nothing to fix.

### Reference


* [ https://www.zaproxy.org/docs/desktop/addons/authentication-helper/session-mgmt-id/ ](https://www.zaproxy.org/docs/desktop/addons/authentication-helper/session-mgmt-id/)



#### Source ID: 3

### [ Storable and Cacheable Content ](https://www.zaproxy.org/docs/alerts/10049/)



##### Informational (Medium)

### Description

The response contents are storable by caching components such as proxy servers, and may be retrieved directly from the cache, rather than from the origin server by the caching servers, in response to similar requests from other users. If the response data is sensitive, personal or user-specific, this may result in sensitive information being leaked. In some cases, this may even result in a user gaining complete control of the session of another user, depending on the configuration of the caching components in use in their environment. This is primarily an issue where "shared" caching servers such as "proxy" caches are configured on the local network. This configuration is typically found in corporate or educational environments, for instance.

* URL: https://tarefa-time-organizador.lovable.app/__l5e/events.270c78a44fc53e7b.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/__l5e/events.270c78a44fc53e7b.js`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `max-age=31536000`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/assets/not-found-DIgawKw1.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/assets/not-found-DIgawKw1.js`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `max-age=31536000`
  * Other Info: ``
* URL: https://tarefa-time-organizador.lovable.app/robots.txt
  * Node Name: `https://tarefa-time-organizador.lovable.app/robots.txt`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: `In the absence of an explicitly specified caching lifetime directive in the response, a liberal lifetime heuristic of 1 year was assumed. This is permitted by rfc7234.`
* URL: https://tarefa-time-organizador.lovable.app/sitemap.xml
  * Node Name: `https://tarefa-time-organizador.lovable.app/sitemap.xml`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: ``
  * Other Info: `In the absence of an explicitly specified caching lifetime directive in the response, a liberal lifetime heuristic of 1 year was assumed. This is permitted by rfc7234.`
* URL: https://tarefa-time-organizador.lovable.app/~flock.js
  * Node Name: `https://tarefa-time-organizador.lovable.app/~flock.js`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `max-age=1500`
  * Other Info: ``

Instances: Systemic


### Solution

Validate that the response does not contain sensitive, personal or user-specific information. If it does, consider the use of the following HTTP response headers, to limit, or prevent the content being stored and retrieved from the cache by another user:
Cache-Control: no-cache, no-store, must-revalidate, private
Pragma: no-cache
Expires: 0
This configuration directs both HTTP 1.0 and HTTP 1.1 compliant caching servers to not store the response, and to not retrieve the response (without validation) from the cache, in response to a similar request.

### Reference


* [ https://datatracker.ietf.org/doc/html/rfc7234 ](https://datatracker.ietf.org/doc/html/rfc7234)
* [ https://datatracker.ietf.org/doc/html/rfc7231 ](https://datatracker.ietf.org/doc/html/rfc7231)
* [ https://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html ](https://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html)


#### CWE Id: [ 524 ](https://cwe.mitre.org/data/definitions/524.html)


#### WASC Id: 13

#### Source ID: 3

### [ Storable but Non-Cacheable Content ](https://www.zaproxy.org/docs/alerts/10049/)



##### Informational (Medium)

### Description

The response contents are storable by caching components such as proxy servers, but will not be retrieved directly from the cache, without validating the request upstream, in response to similar requests from other users.

* URL: https://tarefa-time-organizador.lovable.app/
  * Node Name: `https://tarefa-time-organizador.lovable.app/`
  * Method: `GET`
  * Parameter: ``
  * Attack: ``
  * Evidence: `no-cache`
  * Other Info: ``


Instances: 1

### Solution



### Reference


* [ https://datatracker.ietf.org/doc/html/rfc7234 ](https://datatracker.ietf.org/doc/html/rfc7234)
* [ https://datatracker.ietf.org/doc/html/rfc7231 ](https://datatracker.ietf.org/doc/html/rfc7231)
* [ https://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html ](https://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html)


#### CWE Id: [ 524 ](https://cwe.mitre.org/data/definitions/524.html)


#### WASC Id: 13

#### Source ID: 3


