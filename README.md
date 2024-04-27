## Proxy server for my friends in North America need China network environment:
**No SLA guaranteed** <br>
*VISIT ME IN PERSON IN CALIFORNIA OR BRITISH COLUMBIA.*

## Proxy server for my friends in mainland China:
**No SLA guaranteed** <br>
| Entry 	| Location  	| UDP Type      	| Bandwidth 	| Port  	|
|-------	|-----------	|---------------	|-----------	|-------	|
| IPLC  	| Hong Kong 	| Symmetric NAT 	| 100 Mbps  	| 49151 	|
| 0/2/3 	| Hong Kong 	| Symmetric NAT 	| 200 Mbps  	| 32404 	|
| 0/2/3 	| Macau     	| Symmetric NAT 	| 500 Mbps  	| 38499 	|
| 0/2/3 	| Taipei    	| Symmetric NAT 	| 300 Mbps  	| 32001 	|
| 0/2/3 	| Hong Kong 	| Full Cone NAT*	| 1.2 Gbps  	| 32401 	|
| 0/1/3 	| Tokyo     	| Full Cone NAT*	| 1.8 Gbps  	| 22409 	|
| 0/1/3 	| San Jose  	| Full Cone NAT*	| 2.5 Gbps  	| 22404 	|

## Connection information
Any client with "XUDP" packet encoding are supported, but [mihomo](https://wiki.metacubex.one/) and other GUI implementations are tested. <br>
Use any AES-256-ECB tools with the 27640th block divided by 0x40000 in SDEZ_1.45.00 as KEY, and penultimate 16 byte of SDEZ_I003 as IV. <br>
After that decode the hex with UTF8, you will get the server domain and UUID (or just ask me if I know you). <br>
> 7D 6B 03 E3 9F 6E 91 60 28 91 D1 E5 47 0A 9F 9B <br>
> 50 D2 1B EF 28 31 0D 49 BD 5A BB B1 B0 31 AF AC <br>
> EE 22 B3 ED C6 0E 7C CD FD 4D A9 1F 64 4B 71 1E <br>
> D2 6D 65 79 4A 22 B5 17 7F 1C 52 A3 5E 09 1B 3F <br>
> 61 2F 0E CE 10 E1 17 2D 2E CD 51 A9 EB 25 FB 69 <br>
> 2B 3A 24 1E 83 BD DD 6C 4F 5C 25 22 43 7F B9 5E <br>
> 7E 0E 90 CD C1 1E AE F6 14 8A 2E 6C E8 CE 60 12 <br>
> 2C 15 EA E7 97 83 AF 68 2C 32 00 E9 71 F6 A6 03 <br>
> 40 32 A7 08 82 28 8C 78 0B 37 A3 40 A6 B9 2B CC <br>
> 0A C8 80 5E 38 6E B3 F0 1C DF F5 AC 37 4A F8 31 <br>
> 21 A8 35 41 8A 6E 98 DF 09 A7 56 1E 1C EA B3 4A <br>
> 51 A6 38 D1 77 B4 DB 56 8B 73 3A 47 6E D0 BD 2B <br>
> 47 68 AA 3E 0C 10 69 EF 4A E3 F9 A5 0E 18 6A EE <br>
> 7F 1A 9A CB B5 15 17 DC E2 0A F7 16 D3 95 AA 55 <br>
> DC 8C 94 1F A9 18 62 2B 9C 0D 18 1D A6 91 79 45 <br>
> 72 7C 12 2B EC 87 B9 A8 09 E3 82 0C A5 A1 12 40 <br>

## Extra Notes*
If "UDP Encoding" set to "default" or "None", all server will fallback to "Symmetric NAT" <br>
"Full Cone NAT" require client support "XUDP" packet encoding format, which is NOT part of standard VMess protocol specification. <br>
Server is hosted with Xray v1.8.10, compatible with V2Ray AEAD, but NOT compatible with "PacketAddr" UDP endocing. <br>
You may still connect to server with incompatible UDP encoding clients, just disable them, it will fallback to "Symmetric NAT". <br>

## Entry server selection
0: This is IPv6-Only entry sevrer, which means you will need local IPv6 connectivity to access the relay server, but the actual outbound will always be IPv4-Only. This server has 600 Mbps bandwidth. <br>
1: This is IPv4-Only entry server, with 500 Mbps bandwidth. <br>
2: This is IPv4-Only entry server, with 1000 Mbps bandwidth. <br>
3: This is dual stack entry server, some unresolved SLA issue exist. This server has 800 Mbps bandwidth. <br>
IPLC: This is IPLC server, which has constant 4.5 millisecond latency, ideal for online gaming. This server only has 100 Mbps bandwidth, be kind while using. <br>
> Entry 0 works the best while you have local IPv6 connectivity (usually has lowest usage) <br>
> Entry 3 is least ideal, overall SLA only around 80%, try avoid using it. <br>

## Security
Network activity will never been logged, server-side DoH enabled. <br>
Always check for UDP leak, TCP leak, IPv6 leak, IPv4 leak first before you do anything online. <br>
> Common misconfiguration usually lead to WebRTC leak, DNS leak, Real IPv6 leak. <br>
> You may check [WebRTC here](https://browserleaks.com/webrtc), [DNS here](https://browserleaks.com/dns) and [IPv6 here](https://test-ipv6.com/). <br>
> If you are using my servers, you should never saw your real IP and real DNS in those tests. <br>

## Warning
While using, you shall comply with the legal restrictions of the country of your nationality, as well as the legal restrictions of the country in which you are currently located and the legal restrictions of the location of the proxy server you are using.

*This document is for invited guests only.* <br>