Mario
------

This is a fork of [https://github.com/ded/bowser](https://github.com/ded/bowser).

A Browser detector. Because sometimes, there is no other way, and not even good modern browsers always provide good feature detection mechanisms.

So... it works like this:

``` js
if (mario.msie && mario.version <= 6) {
  alert('Hello China');
}
```

Detected Browsers[Engines]
-----

  * msie
  * safari[webkit]
  * chrome[webkit]
  * firefox[gecko]
  * opera

Detected mobile operating systems
-----

 * android
 * ios (iphone/ipad/ipod)

Android and iOS both report the `osversion` field, containing the OS version number reported in the UA string. Windows Phone is recognized as mobile, is reported as `msie`. Other mobile OS'es (e.g. Blackberry, Windows RT/8) may be added later.

All known mobile OS'es, plus any that report as 'Touch' or similar, will report `touch` as true.

Notes
----
Safari, Chrome, and Firefox will report that they have webkit|gecko engines

``` js
if (mario.webkit) {
  // do stuff with safari & chrome
}
```
