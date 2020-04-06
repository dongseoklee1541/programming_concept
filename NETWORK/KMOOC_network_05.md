# 이동통신과 인터넷프로토콜

## 이동전화와 위성네트워크

### 이동전화(cellur phone)
각 이동전화 서비스영역은 cell 이라 불리는 작은 영역으로 나뉘어짐

* cell ? 기지국이 가상적으로 도달 할 수있는 가상의 영역

* MSC(Mobilc Switching Center) : 이동전화와 기지국과의 관계를 관리

* Handoff : 이동전화가 한 셀에서 다른 셀로 이동(기지국 간의 이동)

### 위성 네트워크
인공위성을 이용한 통신 형태, 2개의 Van Allen 벨트로 인해 세개의 층에 각기 다른 인공위성을 띄움


#### GEO(Geosynchronous Earth Orbit)
정지 궤도 위성으로, 지구의 자전속도와 동일하게 움직임

#### MEO(Medium-Earth Orbit)
2개의 Van Allen 벨트 사이에 위치, GPS(Global Positioning System)로 주로 사용된다.

#### LEO(Low-Earth Orbit)
가장 낮은 위치에 존재하며, 음성통신을 하는데 주로 사용된다.

-----

## 인터넷 프로토콜 : IP

### 네트워크 프로토콜
연결지향 프로토콜과 비연결형 프토콜로 구분된다.

* 연결지향 프로토콜: 데이터를 전송하기 전에 반드시 연결설정을 해야함
* 비연결형 프로토콜 : 연결설정과정 없이**데이터 전송**만이 존재 <-- IP

### IP 패킷의 형태
인터넷 프로토콜인 IP는 비신뢰성(unreliable), 비연결형(connectionless)데이터그램 프로토콜

* best-effort 전달 서비스를 제공
* 에러제어나 흐름제어(수신자를 고려해서 속도 조절)가 없음 -> 다른계층의 프로토콜에서 함 
* 에러 검출만하고 발견되면 폐기

### IP 패킷의 형태

1. 버전(Version : VER) : IP프로토콜의 버전을 나타내는 것, IPv4와 IPv6로 나뉨

2. 헤더의 크기(Header length : HLEN) : 헤더의 크기를 나타내는 것으로 4바이트 단위로 나타낸 크기, 헤더의 크기는 20 ~ 60 바이트로 가변적

3. 서비스 : IP 패킷의 **서비스의 형태**