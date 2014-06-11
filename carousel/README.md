There are certain parameters that can be customized through altering the url of this page and reloading it.

**example url:** http://url.com/example/things/?rs=w&rc=x&fi=y@ci=z

The customizable paramaters are rs=x, rc=x, fi=x, and ci=x

####Parameter Definitions
**rs=x**: after 'x' seconds, refresh the page.  There is a minimum time of five minutes between refresh, entering any number lower than 300 will result in a time of 300 seconds (5 minutes) between refreshes.

**rc=x**: after 'x' number of cycles through the carousel, refresh the page (one cycle consists of each slide in the carousel being shown once).  There is no minimum on the number of cycles required before a refresh.

**fi=x**: The time (in milliseconds) between tweets fading in and out

**ci=x**: The time (in milliseconds) between slide shifts - however if there is a hard-coded slide duration (slideDuration variable in main.js) that number will take precedence.  The code does currently have a hard-coded duration of ---

####Examples
**Base URL:** http://url.com/example/things/

---

**Format for using one parameter:** 

Reloading the page after changing the base url to

url.com/example/things/?rs=x

will set the page to refresh every x seconds

----

**Format for using multiple parameters:**

Reloading the page after changing the base url to

url.com/example/things/?rs=x&fi=y&ci=z

will set the page to refresh every x seconds, sets the time between tweets fading in and out to y milliseconds, and the time between slide shifts to 

----
**Note:** when using rs=x and rc=z at the same time, the page will refresh whenever EITHER of the parameters is met: for example if refresh time is at the minimum of five minutes but z cycles takes one minute, the page will refresh every minute.