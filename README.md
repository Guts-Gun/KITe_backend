# K:ITe 메시지 분배 발송 서비스
 
### 1\. 프로젝트 소개
<img src="https://user-images.githubusercontent.com/114554407/226906763-f450b0c2-6c0e-4260-9ba7-31c839ced1bb.png" width="700"/>
<img width="700"src="https://user-images.githubusercontent.com/114554407/226911661-9ecec86c-13f5-47da-b886-a03d3da5ac67.png">

### 2\. 팀원 소개
| **고솔비**                                                  | **김세빈**                                                      | **이지용**                                                    | **박윤재**                                                          |
|----------------------------------------------------------|--------------------------------------------------------------|------------------------------------------------------------|------------------------------------------------------------------|
| PM,<br>메시지 발송 요청 처리,<br>중계사 비율 분배 및 전송 요청                      | 사용자 주소록 관리,<br>전송에 따른 중계사 응답 처리                              | 전송 결과 상세 통계 조회, <br>더미 중계사 전송 결과 응답                        | 인프라 구축,<br>전송 로그 관리 및 발송 결과 저장                                   |
|https://github.com/solbiko|https://github.com/sbscsue|https://github.com/L-Jiyong|https://github.com/Lab00700|

### 3\. 요구사항 정의

#### 1) 기능 요구사항
1. 대체 발송 기능 : 선택한 발송 실패시 대체 중계사/플랫폼으로 발송
2. 추천 발송 기능 : 중계사별 가격, 속도(실시간) 조회 하여 추천 
3. 주소록 기능 : 주소록 저장 및 그룹별 관리

#### 2) 비기능 요구사항
1. 메세지 전송 : 1000MPS  이상
2. 보안 : bastion host, TLS 인증 통신 암호화
3. 서비스 모듈화 : MSA, k8s pod replica set, 로드밸런싱 트래픽 분산
4. CICD : 빌드 자동화 구현

### 4\. 기술 스택
<img width="700" src="https://user-images.githubusercontent.com/114554407/226910843-a3d45ef7-1bfe-406c-ab37-08891388a40d.png">

### 5\. 프로세스
<img width="700" src="https://user-images.githubusercontent.com/114554407/226910940-e80a8de8-5a46-4a37-88d4-ded7f56aec1b.png">

### 6\. 구현

#### 1) DB
<img width="700" src="https://user-images.githubusercontent.com/114554407/226912100-17fe3868-bf1f-455b-a7af-e15027826b1a.png">

#### 2) MSA
<img width="700" src="https://user-images.githubusercontent.com/114554407/226913877-dd184bd4-9767-48c0-8b33-2b65e81b0957.png">
<img width="700" src="https://user-images.githubusercontent.com/114554407/226913906-ca6aedbc-84d4-4e96-a36f-941c41ce5109.png">
<img width="700" src="https://user-images.githubusercontent.com/114554407/226913911-467bb5c2-9ef8-464f-9b3b-023db20fcb66.png">

#### 3) System Architecture
<img width="700" src="https://user-images.githubusercontent.com/114554407/226911252-35feeb57-fd2d-4cc8-b239-a4c512702453.png">

#### 4)CI/CD
<img width="700" src="https://user-images.githubusercontent.com/114554407/226911075-d8b551ff-66ab-4548-a22f-f8f3858e9b07.png">

### 7\. 프로젝트 관리
<img width="700" src="https://user-images.githubusercontent.com/114554407/226915537-09baa48d-c577-4c61-a73a-005789ec0dde.png">
<img width="700" src="https://user-images.githubusercontent.com/114554407/226915830-eb5f54a1-bd91-43ad-bea6-1c6476e5e42b.png">

### 8\. 소감 및 배운 점
<img width="700" src="https://user-images.githubusercontent.com/114554407/226916388-fd8bbabb-cd53-42c8-bd87-2abc73afe77e.png">

<br><br>
