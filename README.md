
# Few things to consider before getting our hands dirty with a frontend framework:
## 1. Support for Server Side Rendering

SSR is a methodology where the HTML is completely built at the server side and the browser starts rendering the html once it receives the response from the server. Only after rendering the html, the framework (Angular or React) would try to build the virtual DOM and try to attach events to that DOM elements and finally make the page completely interactive.

In case of CSR, after receiving the response from the server, the browser shows a white blank page till it loads all the javascript (including the framework) and it won't render untill it builds the virtual DOM and attaches events to it.

>**Walmart's Electorde** opensource framework is totally all about supporting SSR with much greater performance optimizations. I believe it is totally wrapped over ReactJS.

Another important reason why people would like to do SSR, is to support Search Engine optimizations **SEO**.

## 2. being Cross platform, (May be support for different platforms like Desktop, Mobile and the like?)

An app development framework is said to be Cross Platform when it is written once and executed in multiple platforms or devices like Desktop, Android, Windows Phones, iOS and other exotic platforms like Blackberry 10, LG Web OS, Amazon FireOS.
On installation, the app will show it's widgets with a Native Look and Feel, it will have inherent ability to access Native hardware for different platforms like Camera, GPS and native apps like Calendar, Contacts etc.,

**Apache cordova** (formerly PhoneGap) is the most popular cross platform framework which aids building apps with just HTML, CSS and Javascript.

**Ionic** is another framework that aids in developing hybrid apps.
Ionic is built on top of angular and it needs a Cordova wrapper to access native features like Contacts, Camera and Microphone.
Going for the native UI can sometimes compensate for the performance limitations of browser rendering.

## 3. Support for legacy browsers / browser versions (May be this is where Polyfills are used?)

A polyfill is a piece of code usually javascript which is used to provide modern functionalities on older browsers that do not natively support it.

We can checkout frameworks like **Babel (transpiler+polyfill), Modernizr, core js, polyfill.io** and the like.
