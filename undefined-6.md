# 통합 메시지 전송하기

1.  1\.

    alimtalk 실패 시 sms 발송 (alimtalk,sms)

    insert into msg\_tran(client\_key, channel\_order, request\_date, callback, recipient, kko\_msg\_type, kko\_content, kko\_sender\_key, kko\_template\_code, mt\_content)

    values (sq\_msg\_tran\_01.nextval, 'alimtalk,sms', sysdate, '발신번호', '수신번호', 'AT', 'alimtalk-AT-nobutton 버튼 없는 알림톡 문자 테스트입니다.', '발신프로필키', '템플릿코드', 'sms 문자 테스트입니다.');
2.  2\.

    alimtalk 실패 시 rcs 발송. rcs 실패 시 sms 발송 (alimtalk,rcs,sms)

    insert into msg\_tran(client\_key, channel\_order, request\_date, callback, recipient, kko\_msg\_type, kko\_content, kko\_sender\_key, kko\_template\_code, rcs\_content, rcs\_msgbase\_id, rcs\_brand\_key, mt\_content)

    values (sq\_msg\_tran\_01.nextval, 'alimtalk,rcs,sms', sysdate, '발신번호', '수신번호', 'AT', 'alimtalk-AT-nobutton 버튼 없는 알림톡 문자 테스트입니다.', '발신프로필키', '템플릿코드',

    'RCS\_content입력', 'RCS메시시베이스ID(템플릿코드)', 'RCS브랜드키', 'sms 문자 테스트입니다.(RCS 페일백)');
