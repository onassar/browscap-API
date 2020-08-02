# Browser Capabilities (browscap) API
This repository will document how to use a free hosted `browscap` API to prevent you from having to download and manage the associated INI file yourself.

## Table of Contents
  - [1.00 Proposal](#1.00)
  - [2.00 Endpoints](#2.00)
  - [3.00 Sample Response](#3.00)
  - [4.00 Requests](#4.00)

<a name="1.00"></a>
### [1.00](#1.00) **Proposal**
At the time of documentation (02 August 2020), this document is meant to serve as a proposal for a `browscap` API. If you're interested in this, star this repository and/or please email me ([mailto:onassar@gmail.com](onassar@gmail.com)) to express your interest.

It's in active development, and I hope to have something available soon.


</a><a name="2.00"></a>
### [2.00](#2.00) **Endpoints**
This API will accept two endpoints:

1. https://example.com/api/v1/browser?ua=USER-AGENT-STRING-HERE
2. https://example.com/api/v1/browsers?uas[]=USER-AGENT-STRING-1-HERE&uas[]=USER-AGENT-STRING-2-HERE


</a><a name="3.00"></a>
### [3.00](#3.00) Sample Response
Here is a sample response you can expect:

``` json
{
   "browser_name_regex": "~^mozilla\/5\\.0 \\(.*mac os x.*\\) applewebkit.* \\(.*khtml.*like.*gecko.*\\) .*chrome\/.* safari\/.*$~",
   "browser_name_pattern": "Mozilla\/5.0 (*Mac OS X*) applewebkit* (*khtml*like*gecko*) *Chrome\/* Safari\/*",
   "parent": "Chrome Generic",
   "platform": "MacOSX",
   "comment": "Chrome Generic",
   "browser": "Chrome",
   "browser_maker": "Google Inc",
   "device_type": "Desktop",
   "device_pointing_method": "mouse",
   "version": "0.0",
   "majorver": "0",
   "minorver": "0",
   "ismobiledevice": false,
   "istablet": false,
   "crawler": false
}
```


<a name="4.00"></a>
### [4.00](#4.00) Requests
If you have any requests on endpoints or features to support, please email me:
([mailto:onassar@gmail.com](onassar@gmail.com))
