# Matthew Sigmond

## Daytime

1. 
   1. 1	0.000000000	192.168.119.128	129.6.15.28	TCP	74	48096 → 13 [SYN] Seq=0 Win=64240 Len=0 MSS=1460 SACK_PERM TSval=3008270237 TSecr=0 WS=128
   2. 2	0.039922303	129.6.15.28	192.168.119.128	TCP	60	13 → 48096 [SYN, ACK] Seq=0 Ack=1 Win=64240 Len=0 MSS=1460
   3. 3	0.039948853	192.168.119.128	129.6.15.28	TCP	54	48096 → 13 [ACK] Seq=1 Ack=1 Win=64240 Len=0
2. port 48096
3. it distinguishes between multiple programs using the network
4. 4	0.079683370	129.6.15.28	192.168.119.128	DAYTIME	105	DAYTIME Response
5. "synchronize" and "acknowledge", they are part of the TCP handshake that establishes communication
6. the daytime server, it sent the first packet with the flag "FIN" which terminates communication

## HTTP
1. 2 connections, this is listed under Statistics > Conversations > TCP tab
2. yes, a GET request is sent for / : 

6	0.034751111	192.168.119.128	172.233.221.124	HTTP	439	GET / HTTP/1.1, 

after which the server responds with the page: 

8	0.051827105	172.233.221.124	192.168.119.128	HTTP	669	HTTP/1.1 200 OK  (text/html)

3. similarly, a GET request is setnt for /jeff-square-colorado.jpg:

10	0.074333693	192.168.119.128	172.233.221.124	HTTP	478	GET /jeff-square-colorado.jpg HTTP/1.1 

after which the server responds with the image:

219	0.196629160	172.233.221.124	192.168.119.128	HTTP	692	HTTP/1.1 200 OK  (JPEG JFIF image)

The actual image is sent in packets over TCP and not in one piece, however. 

## Questions

Is there a simple way to stitch together TCP packets to make up an image?

Would HTTPS encrypt what files the client is requesting, or just their contents?