# worker

AGENT의 메시지전송과 관련된 worker에 대한 설명입니다.

#### collector <a href="#collector" id="collector"></a>

* 데이터베이스를 조회하여 발송 대상 데이터를 SEND QUEUE(메모리큐)에 저장한다.

#### sender <a href="#sender" id="sender"></a>

* SEND QUEUE 내부의 데이터를 OMNI 통합메세지 SEND API를 통해 인포뱅크 G/W로 송신한다.

#### receiver <a href="#receiver" id="receiver"></a>

* OMNI 통합메세지 REPORT API를 통해 전송 결과를 수신하여 MSG\_REPORT 테이블에 저장한다.

#### reportMigrator <a href="#reportmigrator" id="reportmigrator"></a>

* TRAN 테이블 데이터에 REPORT 테이블의 데이터 전송 결과를 업데이트한다.

​

* Collector: 데이터베이스를 조회하여 발송 대상 데이터를 SEND QUEUE에 저장
* Sender: SEND QUEUE의 데이터를 OMNI 통합메시지 API를 통해 인포뱅크 G/W로 송신
* Reciever: 리포트 API로 전송 결과를 수신하여 REPORT 테이블에 저장
* ReportMigrator: REPORT 테이블의 데이터를 TRAN 테이블로 이관
* LogMigrator: REPORT 수신이 완료된 TRAN 테이블의 데이터를 LOG 테이블로 이관

​

[PreviousTABLE SCHEMA](broken-reference)[Next- 기능scheduler](broken-reference)

Last modified 12d ago
