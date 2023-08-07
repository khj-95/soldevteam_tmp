# callback

* DB에서 Record 검색 후 사용자 함수를 호출할 수 있도록 인터페이스를 정의하여 제공하고 있습니다.
* 아래 함수는 특정 필드의 값을 가공하기 위해 호출되는 프로세스를 정의한 인터페이스 입니다.
* 사용자가 작성한 class파일(JAVA로 컴파일)을 기본경로 혹은 수정된 경로에 복사하여 적용할 수 있습니다.
  * 기본경로: ib.omni.agent.callback.SampleMTTCallback
  * 경로 수정하기: config/msgConfig 파일의 callback.mtt.class configuration을 원하는 경로로 변경
* 주로 수신번호, 메시지를 암호화하여 사용하거나, 값을 변경하여 전송하고자 할 경우 사용 할 수 있습니다.
