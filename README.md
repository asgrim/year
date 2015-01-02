YaaS
====

Year as a Service. Provides the current year as a service.

* **Current year:** https://raw.github.com/asgrim/year/master/en/currentYear
* **Next year:** https://raw.github.com/asgrim/year/master/en/nextYear
* **Previous year:** https://raw.github.com/asgrim/year/master/en/previousYear

## Examples

### PHP

```php
<?php
$year = file_get_contents('https://raw.github.com/asgrim/year/master/en/currentYear');

echo $year; // 2015
```

### Ruby

```ruby
require 'net/http'
year = Net::HTTP.get_response(URI.parse("https://raw.github.com/asgrim/year/master/en/currentYear")).body
p year # 2015
```

### Python

```python
import urllib2
year = urllib2.urlopen('https://raw.github.com/asgrim/year/master/en/currentYear').read(1000).strip()
print year; # 2015
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

