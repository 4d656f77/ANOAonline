### 프로젝트

![title](https://github.com/4d656f77/ANOAonline/blob/master/images/title.png?raw=true)





# ANOA Gameplay Trailer

[ANOA Gameplay Trailer (ANOA ONLINE) - YouTube](https://www.youtube.com/watch?v=_oR7GiLQZJE)

### 



### 기간/인원/역할

   2022. 10. 11 ~ 2022. 11. 25(7주)

![role](https://github.com/4d656f77/ANOAonline/blob/master/images/role.png?raw=true)

### 



### 기술환경 및 기술 스텍

![architectrue](https://github.com/4d656f77/ANOAonline/blob/master/images/architecture.png?raw=true)

### 



### 구현 서비스 설명

[ANOA ONLINE - ANOA](https://anoa.gitbook.io/anoa-online/anoa/anoa-online)





### 로직

1. 각 클라이언트에서 핑 시스템을 요청한다.

![pressRoger](https://github.com/4d656f77/ANOAonline/blob/master/images/pressRoger.png?raw=true)

    



2.  플레이어의 정보에 접근하는 권한은 서버에 있다.
   
   따라서 지금 플레이어의 컨트롤러가 소유한 캐릭터 위치와 핑 정보를 가지고,
   
   `RPCs`(Remote Procedure Calls)을 이용해서 서버에서 브로드캐스팅 요청한다.

![requestPingSystem](https://github.com/4d656f77/ANOAonline/blob/master/images/requestPingSystem.png?raw=true)

  



3. 서버에서 같은 팀원 리스트에 따라서 개별 클라이언트마다 핑 시스템을 요청한다.

![serverPingSystem](https://github.com/4d656f77/ANOAonline/blob/master/images/serverPingSystem.png?raw=true)





4. 서버에서 요청을 받은 각 클라이언트는 사운드실행과 핑 객체를 생성하고 파괴한다.

![clientPingSystem](https://github.com/4d656f77/ANOAonline/blob/master/images/clientPingSystem.png?raw=true)





5. 본인의 팀에만 확인 객체가 생성되고 사운드가 재생된다.

![ROGER](https://github.com/4d656f77/ANOAonline/blob/master/images/ROGER.png?raw=true)







### 코드

GameMode

![GameMode](https://github.com/4d656f77/ANOAonline/blob/master/images/GameMode.png?raw=true)



GameState

![GameState](https://github.com/4d656f77/ANOAonline/blob/master/images/GameState.png?raw=true)



PlayerController

![PlayerController](https://github.com/4d656f77/ANOAonline/blob/master/images/PlayerController.png?raw=true)



socket

![socket](https://github.com/4d656f77/ANOAonline/blob/master/images/socket.png?raw=true)
