# IP 주소
IP 주소는 네트워크 계층에서 사용하는 주소이며, IP 헤더에 포함된 데이터 주소다.

## IP 주소 유형
IP주소는 진법과 자릿수에 따라 IPv4, IPv6로 나뉘어 진다. 현재는 IPv4에서 IPv6로 옮겨가고 있는 상황이다.

## 서브넷 마스크
서브넷 마스크는 IP주소가 네트워크 아이디와 호스트 아이디를 구별하기 위해서 사용된 것이다. 서브넷 마스크 IP주소는 32bit에 공통 비트 1을 씌워서
네트워크를 표기한다.

* 네트워크 아이디 : 네트워크 아이디가 같다면 같은 네트워크 대역으로 볼 수 있다.

* prefix : 서브넷 마스크 맨 앞의 비트부터 1의 개수를 표기하는 방식을 말함. 서브넷 마스크가 255.255.255.0 이면 맨 앞의 비트부터 1이 24개 있으니
**/24**로 표기한다.

### 네트워크 이름
네트워크 이름은 네트워크 아이디의 호스트 부분이 모두 0인 주소를 말한다. 이 주소는 네트워크를 표기하거나 라우팅 경로로 사용하기 위해서 예약된 값으로 인터페이스 설정이 불가능하다. 

### 서브넷 브로드캐스트 주소
서브넷 브로드캐스트 주소는 네트워크 아이디의 호스트 부분이 모두 1인 주소. 이 주는 네트워크에서 브로드캐스트를 실시할 떄 예약된 값이기 떄문에 인터페이스에 설정이 불가능하다. 

> 예를 들어 192.168.1.1/24 라는 주소의 네트워크 아이디는 192.168.1 이며 뒤에 8비트는 호스트 아이디다. 이 떄 **호스트 아이디 전체가 0인 주소 즉 192.168.1.0 을 네트워크 이름**이라고 한다. 동일한 상황에서 이 때 **호스트 아이디 전체가 1인 주소 192.168.1.255를 서브넷 브로드캐스트 주소**라고 한다.

이 결과 인터페이스에 설정 가능한 IP 주소는 서브넷 마스크의 호스트 아이디에 의해서 정해지는데, 이 때 **사용하지 못하는 네트워크 아이디와 서브넷 브로드캐스트 주소 2개를 뺀 나머지가 사용 가능한 IP주소의 갯수가 된다.**




-------

https://m.blog.naver.com/hatesunny/220790654612
