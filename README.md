# ip-adress-naxva-scapy.arp
ip adress naxva scapy.arp

import scapy.all as scapy


def scan(ip):
    arp_request =scapy.ARP()
    arp_request.pdst = ip
    print(arp_request.summary())
    

scan("10.10.1.1")
