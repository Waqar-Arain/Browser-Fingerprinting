# `Written by Acey:`

Here is the compiled list of some of my findings, based on our topic in #web-app-pentesting.
```
This is a summary of some of the information I found from online searches as well as articles and videos. None of this information is mine, and I could have easily made mistakes. This information could easily become outdated. Please take everything here with a grain of salt xP

```

# PART 1

## GENERAL FINGERPRINTING ARTICLES:

I would be skeptical about this one as many of the facts mentioned are not true and it seems biased towards making fingerprinting sound harder than it actually is, as there are many other ways of fingerprinting that can be used to make a unique fingerprint, and they are not difficult to use at all. 

https://medium.com/slido-dev-blog/we-collected-500-000-browser-fingerprints-here-is-what-we-found-82c319464dc9

https://medium.com/@ravielakshmanan/web-browser-uniqueness-and-fingerprinting-7eac3c381805

https://restoreprivacy.com/browser-fingerprinting/

https://myshadow.org/browser-tracking

https://edu.gcfglobal.org/en/internetsafety/understanding-browser-tracking/1/

https://www.comparitech.com/blog/vpn-privacy/free-anti-tracking-browser-extensions/

https://choosetoencrypt.com/search-encrypt/internet-tracking-why-its-bad-and-how-to-avoid-it/

https://pixelprivacy.com/resources/browser-fingerprinting/

https://www.findyourvpn.com/browser-fingerprinting/


## TEST YOUR BROWSER:

Very popular website to check your fingerprint and test to see if you are unique (within all the fingerprints collected in the last 45 days)

https://panopticlick.eff.org/


Check for DNS and IP leaks (DNS leaks may leak your country if your VPN or Tor isn't configured correctly):

https://www.dnsleaktest.com/
https://ipleak.net/

Am I unique: a website to view basic details of your user agent string in a nice user-friendly way and check if you are unique:
https://www.amiunique.org/

# PART 2

## FINGERPRINTING METHODS:

List of some fingerpriting methods:

IP address
cookies
browsing history
User agent string:
    OS type (windows, linux, android, IOS, OSX, etc)
    OS version
    Language
    Timezone + local time
    Acceptable file formats
    Available audio formats

Browser fingerprint:
- Available fonts
- HTML canvas & rendering
- Do not track requests
- Javascript enabled yes/no
- Cookies enabled yes/no
- location (yes, browsers may allow websites to view your location (they will usually ask permission first!))
- Accelerometer
- Gyroscope
- Adobe flash player info
- Browser plugins


Screen size and resolution
Color depth
CPU model (can be identified by executing a certain piece of code and measuring the time taken to complete (as well as many other ways)
GPU model

# PART 3

## YOUTUBE CHANNELS FOR PRIVACY AND SECURITY
This youtube channel is VERY useful for protecting your privacy online. I reccomend watching as many videos as possible and implementing as many methods as you can: 

https://www.youtube.com/channel/UCjr2bPAyPV7t35MvcgT3W8Q
You can start with this video of his: 

https://www.youtube.com/watch?v=Hjspu7QV7O0 

Personally, I would say this is THE BEST source of privacy advice that exists. I honestly owe so much to this person. He has done so much for all of us by teaching us about the dangers of not protecting our privacy and how to do so. He makes videos that no one else makes because they will not be payed or monetized. He is not afraid to stand up for what's right, even at his own (possibly great) risk. If you do use a youtube account, please subscribe to his channel and like and share his videos so they reach as many people as possible. Don't forget to share information in this post with everyone who may be interested. Also, I suggest implementing some of the techniques that don't sacrifice any functionality for your parents and relatives who don't really care about privacy and security. I have https everywhere and decentraleyes installed for my parents. I also recommend teaching them how to use ublok origin (just press the big power button if the website acts weird).

# PART 4

## BROWSER EXTENSIONS FOR SPOOFING USER AGENT STRING:

### Google chrome:
An extension to change the user agent string with support for multiple common browsers, tablets, google bots, and random mode! This is a basic extension. https://chrome.google.com/webstore/detail/user-agent-switcher-for-c/djflhoibgkdhkhhcedjiklpkjnoahfmg


### Firefox:
An extension to view and set custom user agent strings, as well as support for a large number of mainstream browsers. This is a little more advanced. https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher
*note: if you use a completely custom user agent string, you WILL be unique and fully trackable.

This extension is much and user-friendly: https://addons.mozilla.org/en-US/firefox/addon/uaswitcher

### Extensions availble on all browsers:
https everywhere
Decentraleyes
ublock origin
umatrix
cookie autodelete

I strongly recommend using at least the first 3.BROWSER EXTENSIONS FOR SPOOFING USER AGENT STRING:

### Google chrome:
An extension to change the user agent string with support for multiple common browsers, tablets, google bots, and random mode! This is a basic extension. https://chrome.google.com/webstore/detail/user-agent-switcher-for-c/djflhoibgkdhkhhcedjiklpkjnoahfmg


### Firefox:
An extension to view and set custom user agent strings, as well as support for a large number of mainstream browsers. This is a little more advanced. https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher
*note: if you use a completely custom user agent string, you WILL be unique and fully trackable.

This extension is much and user-friendly: https://addons.mozilla.org/en-US/firefox/addon/uaswitcher

### Extensions availble on all browsers:
https everywhere
Decentraleyes
ublock origin
umatrix
cookie autodelete

I strongly recommend using at least the first 3.
# PART 5

## RELATED: TOR
https://www.torproject.org/

Check if your browser is using tor (must be configured manually xP) https://check.torproject.org/


### Tor browser fingerprinting:

http://jcarlosnorte.com/security/2016/03/06/advanced-tor-browser-fingerprinting.html

https://www.helpnetsecurity.com/2016/03/11/fingerprint-tor-browser-users/

Measures Tor has taken against these methods:

"There are many other changes that have been made to the Tor browser over the years to prevent the unique identification of users. Tor warns users when they maximize their browser window as it is also one attribute that can be used to identify them. It has introduced default fallback fonts to prevent font and canvas fingerprinting. It has all the JS clock sources and event timestamps set to a specific resolution to prevent JS from measuring the time intervals of things like typing to produce a fingerprint."

"Talking about his contribution towards preventing browser fingerprinting, Laperdrix wrote, “As part of the effort to reduce fingerprinting, I also developed a fingerprinting website called FP Central to help Tor developers find fingerprint regressions between different Tor builds.”"

--source: https://hub.packtpub.com/the-tor-project-on-browser-fingerprinting-and-how-it-is-taking-a-stand-against-it/

### Contribute:
submit your tor browser fingerprint on this site, used to study tor browser fingerprints and help developers minimize the differences between them! https://fpcentral.tbb.torproject.org/

DONE! XD

that was a lot xD

I hope it helps you tho and I hope you don't just ignore it xDD