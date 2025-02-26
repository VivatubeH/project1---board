저는 m1 macbook이라 도커를 이용해서 오라클을 설치했습니다. 

IntelliJ에서 DB를 연결하는 방법을 알아봅시다.

<img width="311" alt="image" src="https://github.com/user-attachments/assets/f987e132-5ce8-49a0-9e65-2c5773019676" />

IntelliJ IDE의 우측에서 데이터베이스 아이콘을 클릭해주고 +를 클릭합니다.

<img width="459" alt="image" src="https://github.com/user-attachments/assets/04ec2840-4a11-4161-8898-6e27d21e1b0e" />

DataSource는 오라클 DBMS를 사용할 것이기 때문에 오라클을 선택해줍니다.

```
Host : localhost
Port : 1521
SID : XE 
Username : 오라클에서 생성한 계정 아이디
Password : 오라클에서 생성한 계정 비밀번호
```

-> 참고로 오라클 23c부터는 무료 버전 SID가 FREE로 설정되지만, 저는 21c 버전 오라클을 사용하기 때문에 XE로 입력합니다.

<img width="900" alt="image" src="https://github.com/user-attachments/assets/6136e542-3bae-4010-8a42-a14f6246dcf3" />

오라클 버전 확인은 아래 sql 명령어를 실행하면 확인할 수 있습니다.

```sql
select * from v$version;
```

<img width="775" alt="image" src="https://github.com/user-attachments/assets/500687dc-a1eb-4306-bf46-b36a5237b3da" />

무튼 비밀번호까지 맞다면, succeed가 됩니다. succeeded가 되면 연결이 가능해졌습니다.

<img width="1417" alt="image" src="https://github.com/user-attachments/assets/84c02b1c-2c35-4ced-9112-0b1723b5cb52" />

연결이 되면 위 사진처럼 인텔리제이 내에서 SQL문을 작성하고 테스트할 수 있습니다.
