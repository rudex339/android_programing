# SPGP_Term_Project 
스마트폰 게임 프로그래밍 텀 프로젝트 1차 발표

1. **게임 컨셉**
   
   밀려오는 적들을 아군 타워를 배치하여 막아내자

   
   
2. **진행 상황**
   
|주차|개발 내용|비고|
|---|---|---|
|1주차|게임 프레임 워크 제작|30%|
|2주차|기본 스테이지 클래스 제작|100%|
|3주차|아군 타워 기본 클래스 제작|100%|
|4주차|적 유닛 기본 클래스 제작|100%|
|5주차|스테이지 제작|20%|
|6주차|적 ai 제작, 자원 추가||
|7주차|4가지 종류 타워 제작||
|8주차|4가지 적 유닛 추가||
|9주차|디버그||

![image](https://github.com/rudex339/Sdgp-termproject/assets/58317478/9400b9ac-ce8b-4aac-b5ac-ec321360fd59)


|1주차|2주차|3주차|4주차|5주차|
|---|---|---|---|---|
|3|1|2|0|1|

3. **main sence의 GameObject**

TowerGenerator

![image](https://github.com/rudex339/Sdgp-termproject/assets/58317478/96351a80-64c8-4cd2-8374-5d9cc2c4330f)

  이미 배치된 타일에는 배치가 되면 안되므로 한 클래스에서 관리가 필요

   

  클릭을하면 임의의 타워가 그려지고 손가락을 따라오다가 손가락을 떼면 생성된다
  
  -Tower

  체력, 소모 자원, 공격력
  
    기본 패턴
    
    -타일 위에만 배치가 되며 enemy와 마주친다면 적을 멈추게한후, 공격한다

    -체력이 0이 되면 파괴된다

    원거리 패턴

    -특정 거리내에 적이 있다면 공격한다
  
EnemyGenerator

![image](https://github.com/rudex339/Sdgp-termproject/assets/58317478/3980d501-bdeb-46aa-8b5c-73e14afc04f1)

적을 자동으로 생성하고 웨이브를 관리함

  -Enemy

  체력, 속도, 공격력
  
  기본 패턴
  
  -성을 향해 계속 앞으로 나아간다

  -체력이 0이되면 파괴된다
  
  -타워와 접촉하면 멈추고 공격한다

  원거리 패턴
  
  -주변에 타워가 있다면 특정시간마다 멈춰서 공격한다
  



   
