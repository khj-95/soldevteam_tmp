# ha mode

* 장애가 발생하더라도, 중단없는 서비스를 위해 AGENT 서버 이중화를 제공합니다.
* Active-Active mode, Active-Standby mode 서비스를 제공합니다.
  * Active-Active: 이중화된 Agent가 모두 동작하는 방식
  * Active-Standby: Primary와 Secondary로 구별하여 Primary 서버의 agent가 메인으로 동작하며 서버 장애 시 Secondary 서버가 자동으로 장애를 감지하고 이어서 전송하는 방식
