# About this fork (TinyProxy)
This fork is maintained and built primarily as the backend to a simple proxy app I'm creating called [TinyProxy](https://play.google.com/store/apps/details?id=appinventor.ai_DaProgramerForBatch.BasicWebProxy)
It's purpose isn't really to provide a highly secure or private way of browsing the internet, but really to just be a simple solution to get onto a blocked website. With that being said, if I see a potential privacy or security improvement, I will commit it.

## Changes from MiniProxy
* `<object>` tags are now proxified
* Cookie support in progress (please don't use yet)
* `Referer` header is spoofed. [Originally from here](https://github.com/nkorth/miniProxy)
* Only replace origin header if `$forceCORS` is set to true [Source](https://github.com/nkorth/miniProxy/commit/38b1a992d67d7e744cb13cb13f1a89a1034966a4)
* Sent a DNT (do not track) header whenever `anonymize` is set to `true`

# :rotating_light::warning: Warning: Deprecated/no longer maintained! :warning::rotating_light:

**As of April 26th, 2020, miniProxy is no longer maintained, and no further changes will be made to it (including security-related changes).**

When miniProxy was first released as [PageForward](http://pageforward.sf.net) in 2005, the Internet was dramatically different than it is as of this writing fifteen years later, in 2020.

Since 2005, web standards and web browsers have improved dramatically, both in terms of available functionality and in terms of security for end users.

Over time, those welcome improvements have made it more difficult (and inherently less secure) to maintain and use a web proxy such as miniProxy. miniProxy provides a flawed and subpar browsing experience with the modern web.

I have also had no personal use for miniProxy in quite some time, which caused the effort I put into maintaining it to be minimal at best.

Given all of the above, I believe miniProxy's useful lifetime has now come to an end, and I have decided to stop maintaining it.

This GitHub repository is now archived, but will remain online for future reference for as long as is feasible.

If you continue to use miniProxy, you do so **entirely at your own risk** (as its [GNU GPL v3 license](https://www.gnu.org/licenses/gpl-3.0.html) has always stated, quoted below) and with the understanding that **no web proxy can perfectly anonymize your web browsing.**

> THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
> APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
> HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
> OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
> THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
> PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
> IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
> ALL NECESSARY SERVICING, REPAIR OR CORRECTION.

Thank you for using and contributing to miniProxy and PageForward for the past fifteen years!

-Josh

---

# miniProxy

*by Joshua Dick*

*[http://joshdick.github.io/miniProxy](http://joshdick.github.io/miniProxy)*

---

## About miniProxy

miniProxy is a simple web proxy written in PHP that can allow you to bypass Internet content filters, or to browse the internet anonymously. miniProxy is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.html). miniProxy is the successor to [PageForward](http://pageforward.sf.net).

## Prerequisites

miniProxy should be able to run on any web server with PHP 5.4.7 or later. miniProxy requires PHP's `curl` and `mbstring` extensions to be installed.

## Installation and Use

Simply copy `miniProxy.php` to your web server (it's okay to rename it) and access it directly. That's it! You'll be presented with further usage instructions.

miniProxy doesn't require any configuration out of the box, but configuration options are available; see the top of `miniProxy.php` for details.

## Known Limitations

miniProxy has several known limitations. Some of them may be fixed in future releases. For now, they include:

* No cookie support
* Basic AJAX support, but only for browsers that use `XMLHttpRequest`

## Contact and Feedback

If you'd like to contribute to miniProxy or file a bug or feature request, please visit [its GitHub page](https://github.com/joshdick/miniProxy).

