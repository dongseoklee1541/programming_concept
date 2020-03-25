# LAN 매체와 유선 LAN


전송 매체는 에너지를 전달하는 물질을 의미한다. (송신자와 수신자의 중간다리 역할)

## 전송매체의 종류
종류는 유선(유도체,Guided wried), 무선(비유도체,Unguided)가 있다.

#### 유도매체

* Twisted-Pair Cable : TP 케이블은 두 개의 도체가 절연체로 감싸고 꼬인 것을 의미
  * UTP : Unshielded Twisted-Pair, 외부로 부터의 잡음을 막아줌
  * STP : Shielded Twisted-Pair, 외부 잡음의 침투를 막기 위해 차폐시킨 것
  
* TP 커넥터 : TP케이블을 연결하는 커넥터, RJ가 붙어있는걸 주로 사용한다

* 동축 케이블 : 케이블 티비에 사용되는 선, 높은 주파수의 신호를 전달 할 수 있지만, 멀리갈수록 신호가 약해진다.

* 광 케이블


#### 비유도매체

* 물리적인 도체 없이 신호를 전달하는 매체 : 공기에다가 주파수를 삐슝삐슝 쏜다.



# 유선 LAN : Ethernet

이더넷은 LLC와 MAC으로 구성된 2개의 부계층이 존재

### MAC 계층
매체의 특성과 운용방식에 따라 여러 개의 프로토콜이 존재
* 이더넷 프레임은 7개의 필드로 구성됨
  * CRC(Cyclical Redundancy Check) : 사용자가 보내는 데이터 부분에 에러가 있느냐 없느냐를 확인하는데 사용되는 필드

### LLC(Logical Link Control)
미디어 엑서스 컨트롤(MAC)하는 프로토콜의 종류와 상관없이 공통적으로 가져야할 기능들을 모아놓은 것이 "LLC"다. LAN에서 흐름제어, 에러제어 등 각종 제어에 대한 행위를 수행한다.

#### 주소 지정
각 시스템은 NIC(Network Interface Card)를 갖고 있는데, LAN 카드라고도 불린다. 
 * LAN카드에는 고유 주소가 있는데, MAC주소(Ethernet주소, 하드웨어 주소)라고 한다.