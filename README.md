# Python-notes 19 Feb 2024

## Browser
- Only understand HTML, CSS and JS. All code gets transformed to these languages.
- Mosaic was the first ever web browser.

## Web Apps
- Has front-end, back-end/server and database.
- The following happens when you type google.com:

## IP 
- IPv4 has 32-bit address sizes, has +-4.2 billion addresses and uses dotted decimal notation.
- IPv6 has 128-bit address sizes,
- ISPs assign public IP addresses. 
- Private IP addresses are unique to each device and are assigned by routers.
- Dynamic IP addresses are assigned to a device that needs an IP address whenever it is available. 
- Static IP addresses are reserved for specific users.
- MAC address

## Connections
- TCP is the transmission control protocol and it makes sure that a connection is established. It is unicast and more reliable than UDP while being slower. Used for email and web browsing.
- UDP does not ensure the connection before sending data. It is faster but without guaranteed transfers. Used for live streaming, online games and VoIP. Can be multicast, unicast and broadcast.
- HTTP when you click on a link in your web browser, it’s HTTP that facilitates the retrieval of the linked content from a web server. HTTP is fundamental to our web browsing experience, enabling seamless access to information across the internet.
- HTTPS is asecure variant of HTTP, called HTTPS, is used by over 85% of websites. It encrypts data transmission, enhancing security.
- HTTP3 builds on UDP instead of TCP. Only supports encrypted connections due to the integrated TSL 1.3 encryption. HTTP3 foregoes an additional encryption request (handshakes) at the TLS level, and thus avoids unnecessary security queries. 
- Head-of-line blocking is a network latency bottleneck that occurs when one request blocks another from completing. HTTP/3 is a relatively straightforward adaptation of HTTP/2 running over QUIC, which is built atop UDP. UDP does not guarantee delivery and no dependencies among segments, which means no more head-of-line blocking.

## MDN Status Codes
- 200: Success.
- 300: Redirect.
- 400: User error.
- 500: Server error.

## Document Object Model
- The DOM is a W3C (World Wide Web Consortium) standard that provides a platform and language-neutral interface for programs and scripts to dynamically access and update the content, structure, and style of an HTML or XML document.
- Connects web pages to scripts or programming languages by representing the structure of a document—such as the HTML representing a web page—in memory.
- HTML => HTML Parser => DOM
- CSS => CSS Parser => CSSOM
- JS => JS Engine => DOM/CSSOM

## CSS Terms
```
p, div{
    Color: pink
}

.error{
    backgroud: red
}
```

- From curly brace to curly brace is a declaration block. 
- A single line in a block is a declaration. 
- "background" is a property.
- "p, div" is a selector.
- The whole thing is a rule. 
- ".error" is a class selector.

## Structure of a Web Browser
- User interface(back, forwards, refresh buttons etc) => [Browser Engine(delegate to the rendering or the JS engine), Rendering Engine(has the parsers, create the rendering tree)] => JS engine (handles JS rendering that can't be handled by the rendering engine.)
- Data storage has arrow coming from Rendering engine. UI backend(determines the styles of the UI). Arrow comes fron User interface.
- One more thing missing

- A cache is a copy of the actual data, kept closer to where it is needed. Fast access, not permanent.

## Web App VS Native App
- Web Apps can be accessed through the device’s Web browser, Web Apps are based on internet-enabled applications. In order to access we don’t need to download and install the app onto a mobile device.
- A single web app can be used on most devices capable of surfing the web, it does not depend upon the operating system they use.

### Advantages
- Web apps function in-browser, so they do not need to be installed or downloaded.
- Web apps are easy to maintain, as they have a common codebase regardless of the operating system.
- Can be set to update themselves automatically.
- Easier and faster to build than native mobile apps.
- App store approval is not required, so web apps can be launched easily.

### Disadvantages
- Web Apps do not work without an internet connection.
- Slower than mobile apps.
- It is difficult to discover web apps since they aren’t hosted in a specific database like an app store.
- Web apps have higher risks and poor quality, and there is no guarantee of security since web apps don’t need to be approved by the app stores.

## Web App VS Website
- Web application is designed for interaction with end users.
- Website basically contains static content.

## Python Fundementals

- Use input() to capture user input.
- Interpolation does automation conversion to strings. ({f}).
- Python has 0 based indexes. End value is not inclusive.
- String literals are immutable.

### Data types
- Do not have to delcare a data type.
- Type() returns the datatype.
- Need an underscore when declaring Booleans(e.g is_Young). True and False begin with capital letters. 
- String, int, float, boolean.

### Type Conversion
- user type() to convert. E.g x = str(Y) or x = float(Y).

### Arithmetic Operators
- +, -, *, /, %.
- ** (exponentiation), // (Floor division).