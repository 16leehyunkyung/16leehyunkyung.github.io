---
layout: post
title: 간단한 이체 프로그램
---

<img src="/assets/images/bank_code.PNG" width="30%" height="20%">

계좌의 소유주 변수를 선언해줬다.
_owner 매개 변수를 받아 계좌소유주인 owner에 넣어줬다.


deposit() - 입금함수
이 함수는 payable함수 이므로 직접적으로 이더리움을 전송해서 트랜잭션이 가능하다.
require를 이용해 괄호 안의 값을 이용해 참 거짓을 판명낸다. 
참일 경우에는 계속 실행한다. 

msg.value(전송하는 이더리움의 양) > 0 은 입금 금액이 0 eth이상인가?를 확인해준다.

withdraw() - 출금함수
require를 이용해 보내는 사람과 계좌 소유주가 같은 가?를 확인해준다.
transfer함수는 괄호 안의 양만큼 이더리움을 송금하는 함수이다.

balance는 계좌의 잔고이므로 잔고만큼 owner에게 송금한다.


<img src="/assets/images/bank_deploy_migrate.PNG" width="30%" height="20%">
<img src="/assets/images/bank_compile.PNG" width="30%" height="20%">
<img src="/assets/images/bank_compile2.PNG" width="30%" height="20%">
<img src="/assets/images/bank_deploy.PNG" width="30%" height="20%">
<img src="/assets/images/bank_owner.PNG">
<img src="/assets/images/bank_gana.PNG">