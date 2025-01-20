YaaS
====

Year as a Service. Providing you with extremely accurate year as an API service, since 2015.

* **Current year:** https://raw.github.com/asgrim/year/master/en/currentYear
* **Next year:** https://raw.github.com/asgrim/year/master/en/nextYear
* **Previous year:** https://raw.github.com/asgrim/year/master/en/previousYear

## Examples

Note that these examples may not take into account good security practices, for example escaping output to prevent XSS vulnerabilities.

### PHP

```php
<?php
$year = file_get_contents('https://raw.github.com/asgrim/year/master/en/currentYear');

echo $year; // 2025
```

### Ruby

```ruby
require 'net/http'
year = Net::HTTP.get_response(URI.parse("https://raw.github.com/asgrim/year/master/en/currentYear")).body
p year # 2025
```

### Python

```python
import urllib2
year = urllib2.urlopen('https://raw.github.com/asgrim/year/master/en/currentYear').read(1000).strip()
print year; # 2025
```
### JavaScript

```javascript
// Fetch
fetch('https://raw.githubusercontent.com/asgrim/year/master/en/currentYear')
    .then(resp => resp.json())
    .then(year => console.log(year)) // 2025

// XMLHttpRequest
let xhr = new XMLHttpRequest()
xhr.open('GET', 'https://raw.githubusercontent.com/asgrim/year/master/en/currentYear', true);
xhr.onload = () => {
    if (xhr.status >= 200 && xhr.status < 300 || xhr.status === 304) {
        console.log(xhr.responseText)
    }
};
xhr.send(); // 2020
```
### Bash

```Bash
#!/bin/bash
## Fetch
page="$(curl -s https://raw.githubusercontent.com/asgrim/year/master/en/currentYear)"
echo "$page" # 2025

```
## BC Break

In the future, we may have to break BC by removing the root "[currentYear](https://raw.github.com/asgrim/year/master/currentYear)". You should use "[en/currentYear](https://raw.github.com/asgrim/year/master/en/currentYear)" instead.

## Internationalisation (i18n)

YaaS also supports the following calendars:

Hebrew (he):

* **Current year:** https://raw.github.com/asgrim/year/master/he/currentYear
* **Next year:** https://raw.github.com/asgrim/year/master/he/nextYear
* **Previous year:** https://raw.github.com/asgrim/year/master/he/previousYear

Chinese (zh-cn):

* **Current year:** https://raw.github.com/asgrim/year/master/zh-cn/currentYear
* **Next year:** https://raw.github.com/asgrim/year/master/zh-cn/nextYear
* **Previous year:** https://raw.github.com/asgrim/year/master/zh-cn/previousYear

## FAQs

**Should I use this in my real application?**
* No.

**r u troleing me?**
* Yes.
