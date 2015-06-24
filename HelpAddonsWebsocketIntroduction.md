# WebSockets #

WebSockets can be used by web applications or web sites to setup a bi-directional (two-way), full duplex communication channel over a single TCP connection.
It features a lightweight protocol, allowing developers to realize realtime use cases. WebSockets do also provide an alternative to heavy use of Ajax, HTTP Long Polling or Comet.


After an initial HTTP based handshake, the TCP connection is kept open, allowing applications to send & receive arbitrary data. Often port 80 or 443 for encrypted WebSocket channels are used.

The WebSocket standard is defined in

[The WebSocket API (http://www.w3.org/TR/websockets/)][The WebSocket API _http_www.w3.org_TR_websockets]

specifies the interface in browsers

[The WebSocket Protocol (RFC6455) (https://tools.ietf.org/html/rfc6455)][The WebSocket Protocol _RFC6455_ _https_tools.ietf.org_html_rfc6455]

describes the structure of WebSocket frames upon TCP

ZAP is able to:

 *  intercept and show WebSocket messages
 *  set breakpoints on specific types of WebSocket messages
 *  fuzz WebSocket messages (send lots of invalid or unexpected data to a browser or server)

WebSocket messages are displayed within the [WebSockets tab][].


[The WebSocket API _http_www.w3.org_TR_websockets]: http://www.w3.org/TR/websockets/
[The WebSocket Protocol _RFC6455_ _https_tools.ietf.org_html_rfc6455]: https://tools.ietf.org/html/rfc6455
[WebSockets tab]: HelpAddonsWebsocketTab