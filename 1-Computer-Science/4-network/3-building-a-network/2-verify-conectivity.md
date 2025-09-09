# Verify Connectivity



Every device that sends messages across the internet must have an Internet Protocol (IP) address to identify it to the other devices in the network. IP addresses are assigned by network administrators. When a new device is added to a network, or if an existing device is having problems, it may be necessary to test the network to determine if the IP address assigned to the device can be reached by other devices on the network.

The ping utility tests end-to-end connectivity between the IP address of the source of the message and the IP address of its destination. It measures the time that it takes test messages to make a round trip from the source to the destination, and whether the transmission is successful. However, if the test message does not reach the destination, or if delays are encountered along the way, there is no way to determine where the problem is located.

The format of the ping command is universally implemented. Almost all network attached devices provide a way to perform a ping test. The format of the ping command is ping x.x.x.x, where x.x.x.x is an IP address or domain name: For example, **ping 192.168.30.1.**



## The Traceroute Command

The internet is not really a place; it is the interconnection of many different networks that provide services to the users. We can see this connectivity by using a network utility called **traceroute.**

The traceroute utility traces the route a message takes from its source to the destination. Each individual network through which the message travels is referred to as a hop. The **traceroute** command displays each hop along the way and the time it takes for the message to get to that network and back.

To install it on linux we use

```bash
sudo apt install traceroute
```



We can type the IP or the DNS in order to trace the route of a package.

```bash
traceroute www.google.com
#Output
traceroute to www.google.com (142.250.65.132), 30 hops max, 60 byte packets
 1  speedport.ip (192.168.1.254)  5.909 ms  5.891 ms  5.879 ms
 2  ipdsl-ags-vinedo-14-l0.uninet.net.mx (201.154.85.110)  37.595 ms  37.606 ms  37.596 ms
 3  reg-qro-triara-48-ae0.0.uninet.net.mx (189.246.170.93)  37.588 ms  37.579 ms  37.528 ms
 4  72.14.242.160 (72.14.242.160)  40.517 ms  42.140 ms  43.253 ms
 5  * * *
 6  qro01s25-in-f4.1e100.net (142.250.65.132)  50.340 ms 142.250.210.158 (142.250.210.158)  51.271 ms 142.251.78.182 (142.251.78.182)  51.217 ms

```

El comando "traceroute" y el  comando "Ping" nos ayudarán a saber cuando haya un problema en la red, debido a que si hay un problema de conexión podrás detectar donde está. 

En caso de traceroute, el paquete viajará por varios routers hasta llegar a su destino, si en un router hay un error solo es cuestión de saber su IP y ver cual es el problema de este router. 

En el caso del código Ping si hay un problema de conexión es más fácil, debido a que es en la misma red y solo es cuestión de revisar la red

```bash
ping www.google.com
PING www.google.com(qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004)) 56 data bytes
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=1 ttl=112 time=36.5 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=2 ttl=112 time=30.0 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=3 ttl=112 time=30.8 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=4 ttl=112 time=34.2 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=5 ttl=112 time=45.5 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=6 ttl=112 time=48.2 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=7 ttl=112 time=42.1 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=8 ttl=112 time=31.2 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=9 ttl=112 time=29.6 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=10 ttl=112 time=50.3 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=11 ttl=112 time=29.1 ms
64 bytes from qro02s27-in-x04.1e100.net (2607:f8b0:4012:819::2004): icmp_seq=12 ttl=112 time=28.7 ms
^C
--- www.google.com ping statistics ---
12 packets transmitted, 12 received, 0% packet loss, time 11015ms
rtt min/avg/max/mdev = 28.652/36.343/50.275/7.699 ms

```

