# TABLE SCHEMA

CLIENT\_KEY

NUMBER(20,0)

No

​

클라이언트 메시지 고유 번호

MSG\_KEY

VARCHAR2(40 BYTE)

Yes

​

메시지 키

PAYMENT\_CODE

VARCHAR2(20 BYTE)

Yes

​

정산용 부서코드

PRIORITY

VARCHAR2(10 BYTE)

Yes

'slow'

전송 우선 순위

(veryfast > fast > slow)

CHANNEL\_ORDER

VARCHAR2(80 BYTE)

No

​

전송 채널 순서(fallback 포함)

(예:alimtalk,rcs,sms)

MSG\_STATUS

VARCHAR2(1 BYTE)

No

'1'

메시지 상태

1:발송대기

2:발송완료

3:완료

REQUEST\_DATE

TIMESTAMP(6)

No

​

전송 요청 시간

CALLBACK

VARCHAR2(30 BYTE)

Yes

​

발신번호

(문자나 RCS 발송 시 필수)

RECIPIENT

VARCHAR2(30 BYTE)

No

​

수신번호 (국제표준)

MSG\_SENT\_DATE

TIMESTAMP(6)

Yes

​

발송 요청 시간(Agent가 G/W 로 발송한 시간)

AGENT\_ID

VARCHAR2(2 BYTE)

Yes

' '

AGENT 이중화시 사용되는 ID

MT\_SUBJECT

VARCHAR2(60 BYTE)

Yes

​

문자 제목 입력정보

MT\_CONTENT

VARCHAR2(4000 BYTE)

Yes

​

문자 내용 입력정보

MT\_FILE\_KEY

VARCHAR2(200 BYTE)

Yes

​

문자 파일키 입력정보

KKO\_MSG\_TYPE

VARCHAR2(2 BYTE)

Yes

​

카카오 메시지 타입

알림톡-AT,AI

친구톡-FT,FI,FW

KKO\_CONTENT

VARCHAR2(4000 BYTE)

Yes

​

카카오 내용 입력정보

KKO\_OPTION

VARCHAR2(4000 BYTE)

Yes

​

카카오 옵션 입력정보(json형태) - 강조문구, 버튼 등

KKO\_SENDER\_KEY

VARCHAR2(40 BYTE)

Yes

​

카카오 알림톡 발신 프로필 키

KKO\_TEMPLATE\_CODE

VARCHAR2(50 BYTE)

Yes

​

카카오 알림톡 메시지 유형 템플릿 코드

RCS\_CONTENT

VARCHAR2(4000 BYTE)

Yes

​

RCS 내용 입력정보(json형태) - Standalone, Carousel, Template

RCS\_OPTION

VARCHAR2(4000 BYTE)

Yes

​

RCS 옵션 입력정보(json형태) - header, footer 등

RCS\_BRAND\_KEY

VARCHAR2(64 BYTE)

Yes

​

생성한 브랜드마다 부여되는 Key

RCS\_AGENCY\_KEY

VARCHAR2(64 BYTE)

Yes

​

대행사 key

RCS\_MSGBASE\_ID

VARCHAR2(40 BYTE)

Yes

​

RCS 메시지베이스 ID(템플릿코드)

TTL

NUMBER

Yes

​

전송 유효 시간(단위, 초)

ORIGIN\_CID

VARCHAR2(20 BYTE)

Yes

​

발신자 식별코드

MTR\_MESSAGE\_TYPE

VARCHAR2(10 BYTE)

Yes

​

MT 상세 메시지 타입

(sm/lm/mm/im)

MT\_RSLT\_DATE

TIMESTAMP(6)

Yes

​

MT 단말기 도착 시간

MT\_REPORT\_DATE

TIMESTAMP(6)

Yes

​

MT 인포뱅크로부터 결과 수신한 시간

MT\_REPORT\_CODE

VARCHAR2(10 BYTE)

Yes

​

MT 전송 결과

MT\_TELECOM

VARCHAR2(10 BYTE)

Yes

​

MT 착신망 정보10000-etc

10001-skt

10002-kt

10003-lgu

10006-internet number

10010-safety number

MT\_RES\_CNT

NUMBER

Yes

​

MT 분할 발송 된 결과 값에 대한 건수 (국제 발송)

MT\_DLR\_REPORT\_CODE

VARCHAR2(10 BYTE)

Yes

​

MT DLR 리포트 결과 코드(국제발송)

MT\_DLR\_REPORT\_DATE

TIMESTAMP(6)

Yes

​

MT DLR 리포트 수신 시각(국제발송)

KKOR\_MESSAGE\_TYPE

VARCHAR2(10 BYTE)

Yes

​

카카오 상세 메시지 타입

(at/ai/ft/fi/fw)

KKO\_RSLT\_DATE

TIMESTAMP(6)

Yes

​

KAKAO 단말기 도착 시간

KKO\_REPORT\_DATE

TIMESTAMP(6)

Yes

​

KAKAO 인포뱅크로부터 결과 수신한 시간

KKO\_REPORT\_CODE

VARCHAR2(10 BYTE)

Yes

​

KAKAO 전송 결과

RCSR\_MESSAGE\_TYPE

VARCHAR2(10 BYTE)

Yes

​

RCS 상세 메시지 타입

(rs/rl/rm/rt/ri)

RCS\_RSLT\_DATE

TIMESTAMP(6)

Yes

​

RCS 단말기 도착 시간

RCS\_REPORT\_DATE

TIMESTAMP(6)

Yes

​

RCS 인포뱅크로부터 결과 수신한 시간

RCS\_REPORT\_CODE

VARCHAR2(10 BYTE)

Yes

​

RCS 전송 결과

RCS\_TELECOM

VARCHAR2(10 BYTE)

Yes

​

RCS 착신망 정보10000-etc

10001-skt

10002-kt

10003-lgu

10006-internet number

10010-safety number

REG\_DATE

TIMESTAMP(6)

Yes

sysdate

데이터 등록일자

ETC\_TEXT\_1

VARCHAR2(100 BYTE)

Yes

​

유저 기타필드1

ETC\_TEXT\_2

VARCHAR2(100 BYTE)

Yes

​

유저 기타필드2

ETC\_TEXT\_3

VARCHAR2(100 BYTE)

Yes

​

유저 기타필드3
