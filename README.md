YaaS
====

Year as a Service. Provides the current year as a service.

* **Current year:** https://raw.github.com/asgrim/year/master/currentYear
* **Next year:** https://raw.github.com/asgrim/year/master/nextYear
* **Previous year:** https://raw.github.com/asgrim/year/master/previousYear

Example usage:

```php
<?php

$year = file_get_contents('https://raw.github.com/asgrim/year/master/currentYear');

echo $year; // 2014
```
