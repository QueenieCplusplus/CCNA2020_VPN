# CCNA2020_VPN
Virtual Private Network 虛擬私有網路
取代傳統昂貴得 PVC (Permanent Virtual Connection) 服務。

![vpn](https://raw.githubusercontent.com/QueenieCplusplus/CCNA2020_VPN/master/vpn.png)

# P2P (Peer to Peer) BT, Bit Torrent

此功能稱為『位元洪流』，常常搭配 VPN 產品一起販售，
主要是作用於應用層，非點對點協定，而是人群對人群協定，
當越多人下載檔案時，速度越快。

原理：種子檔案中有 tracker 內容，能解析上傳者的 IP 位址，下載完畢後，也會成為此架構中的上傳者，
讓傳統的伺服器不必獨當一面的面對所有下載需求。


# P2P (Point to Point), 點對點傳輸

藉由 GRE 封裝技術，建構虛擬隧道，實現點對點傳輸。


# Tunneling, 隧道協議

遠端使用者利用 ISP 提供的撥接服務（取代傳統的長途撥接），藉由隧道協定，穿過 WAN ，到達本地端的 LAN 區域網路內。

# 串連方式

可以與 ISP 或是電信公司提供的服務相互合作，不受限制。
如數據機抑或 ADSL，ATM、FrameRelay 亦可! 

# 網速受限

傳統的 PVC 因為基於昂貴設備基礎建設和專線，保證了不受限制的網速，
但是現代的 VPN 是共享線路（與 ISP 租賃撥接服務），無法保證網速。



