# HTTP3
- Just like the previous versions, it is a protocol that allows for communication between different systems. Most commonly used for transferring data from a web server to a browser to view web pages.
- Unlike previous versions, HTTP/3 does not rely on TCP. HTTP/3 uses QUIC, which is a multiplexed(a method for combining multiple analog or digital signals into one signal over a shared medium.) transport layer network protocol built on UDP (User Datagram Protocol).
- Uses the same the same request methods, status codes, and message fields as previous versions.
- Ensures the connection using a QUIC handshake, instead of TCP.
- Advantages over previous HTTP versions include lower latency and faster load times.
- Biggest change and advantage it has over HTTP2 is fixing the "head-of-line blocking" problem.
- Head-of-line blocking is a performance-limiting problem, it occurs when a line of packets is blocked in a queue by a first packet. In other words, it is a bottleneck that occurs when one request blocks another from completing.
-  HTTP3 does not suffer from this bottleneck because it uses QUIC and UDP, since UDP does not guarantee delivery among packets it means that no requests will block each other.
