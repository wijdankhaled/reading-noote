# LOCAL STORAGE
ersistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.

**potentially dealbreaking downsides**
1.  Cookies are included with every HTTP request, thereby slowing down your web application by needlessly  transmitting the same data over and over
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

**What we really want is**
- a lot of storage space
- on the client
- that persists beyond a page refresh
- and isn’t transmitted to the server

### INTRODUCING HTML5 STORAGE
What I will refer to as “HTML5 Storage” is a specification named[ Web Storage](https://html.spec.whatwg.org/multipage/webstorage.html), which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons.

**USING HTML5 STORAGE**
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a strin

![](https://i2.wp.com/programmingwithmosh.com/wp-content/uploads/2018/12/localstorage3.gif?fit=600%2C299&ssl=1)

**TRACKING CHANGES TO THE HTML5 STORAGE AREA**
-  setItem()
- removeItem()
-  clear()

**LIMITATIONS IN CURRENT BROWSERS**
 limitations of the now-standardized HTML5 Storage. I’ll give you the answers first, then explain them. The answers, in order of importance, are “5 megabytes,” “QUOTA_EXCEEDED_ERR,” and “no.”

“5 megabytes” is how much storage space each origin gets by default. This is surprisingly consistent across browsers, although it is phrased as no more than a suggestion in the HTML5 Storage specification. 

#### BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
hile the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy. A new API has been standardized and implemented across all major browsers, platforms, and devices. As a web developer, that’s just not something you see every day, is it? But there is more to life than “5 megabytes of named key/value pairs,” and the future of persistent local storage is… how shall I put it… well, there are competing visions.

**BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS**

While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy. A new API has been standardized and implemented across all major browsers, platforms, and devices. As a web developer, that’s just not something you see every day, is it? But there is more to life than “5 megabytes of named key/value pairs,” and the future of persistent local storage is… how shall I put it… well, there are competing visio