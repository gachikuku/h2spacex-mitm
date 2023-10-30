# H2SpaceX
HTTP/2 Single Packet Attack (Race Condition) low level library based on Scapy

# TODO

- Single Packet Attack - POST &...
  - [x] implement
  - [ ] test functionality on different H2 frameworks
- Single Packet Attack - GET
  - [ ] implement
  - [ ] Content-Length: 1 Method
  - [ ] POST Request with x-override-method: GET header
  - [ ] test functionality on different H2 frameworks
- Threading Response Parsing
  - [ ] implement

# Installation
H2SpaceX works with Python 3 (preferred: >=3.10)

    pip install h2spacex

# Quick Start
You can import the HTTP/2 TLS Connection and set up the connection. After setting up the connection, you can do other things:

```python
from h2spacex import H2OnTlsConnection

h2_conn = H2OnTlsConnection(
    hostname='http2.github.io',
    port_number=443
)

h2_conn.setup_connection()
...
```
see more examples in [Wiki Page](https://github.com/nxenon/h2spacex/wiki/Quick-Start-Examples)

# References & Resources

- [James Kettle DEF CON 31 Presentation](https://youtu.be/tKJzsaB1ZvI?si=6uAuzOt3wjnEGYP6)
- [Portswigger Research Page](https://portswigger.net/research/smashing-the-state-machine#single-packet-attack)
- [HTTP/2 in Action Book](https://www.manning.com/books/http2-in-action)

I also got some ideas from a previous developed library [h2tinker](https://github.com/kspar/h2tinker).

Finally, thanks again to James Kettle for directly helping and pointing some other techniques.
