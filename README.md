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


# L2 P2P (Point to Point), 第二層的點對點傳輸

藉由封裝技術，改變封包，讓封包如同膠囊，彼此建構虛擬隧道，實現點對點傳輸。

* PPP:

封裝技術為 GRE。
鑑別技術則為 RAP、CHAP (爾後發展了 X.509)，加密技術為 DES。
金鑰管理技術則為 SKMIP。


* L2TP:

與 PPP 類同，但是使用 UDP 取代 TCP，能節省通道，可在同一通道實行多條連線傳輸。
比 PPTP 多了 L2TF 技術。

# IPsec (L3), 第三層的點對點傳輸協議

封裝技術為 GRE。
鑑別技術則為 AH (爾後發展了 X.509)，加密技術為 ESP。
金鑰管理技術則為 ISAKMP 框架 + OAKLEY。


# GRE 封裝技術

微軟作業系統則有內建 MPPE，於此技術原理相同。

![gre](https://raw.githubusercontent.com/QueenieCplusplus/CCNA2020_VPN/master/GRE%20Frame.png)


# SetUp 設定方式

![setup](https://raw.githubusercontent.com/QueenieCplusplus/CCNA2020_VPN/master/GUI%20setup.png)


# Tunneling, 隧道協議

遠端使用者利用 ISP 提供的撥接服務（取代傳統的長途撥接），藉由隧道協定，穿過 WAN ，到達本地端的 LAN 區域網路內。
抑或是子公司與母公司需要跨 WAN 對 LANs 進行串接。

# Connection, 串連方式

可以與 ISP 或是電信公司提供的服務相互合作，不受限制。
如數據機抑或 ADSL，ATM、FrameRelay 亦可! 

# Throuput, 網速受限

傳統的 PVC 因為基於昂貴設備基礎建設和專線，保證了不受限制的網速，
但是現代的 VPN 是共享線路（與 ISP 租賃撥接服務），無法保證網速。

# Security, 安全度

專線擁有實體上的安全，而 VPN 的安全度歸功於加密技術。





