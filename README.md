#deprecated
this api is deprecated and unmaintained, i suggest you check out https://github.com/Stichoza/google-translate-php instead.

# Warning
At 2016-01-18, i noticed that Google has changed something with their Javascritp API, which renders this api useless until it is updated.
at the very least, they changed the "tk" algorithm, and as always, the algorithm is highly obfucated and scattered, making it a difficult task to reconstruct and re-implement the algorithm.. see this page for mor information: https://github.com/divinity76/free_google_translate.inc.php/issues/1
# free_google_translate.inc.php
free (no subscription required) google translate api for PHP.
usage: 
```php
  require_once('free_google_translate.inc.php');
	echo free_google_translate("this is a test message","en","no");
```
^ will translate "this is a test message" from english to norwegian. documentation on languages is currently lacking - feel free to contribute! currently known:

Language  | Codename
------------- | -------------
English  | en
Japanese  | ja (NOT jp, as one might expect)
Polish | pl

(know that most languages is what you'd expect, and finding all languages is easy with studying https://translate.google.com/ - i am just being lazy in documentation here.)

#Warning
This API could break at any time. if you need a reliable API, consider https://cloud.google.com/translate/v2/pricing -  
this use an undocumented, reverse-engineered API, the same API that is used by google's own HTML5 client at https://translate.google.com , and it is not affiliated with google in any way, thus this API could break at any time google decide to change something :)
