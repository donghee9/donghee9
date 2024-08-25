## 백엔드 개발자 서동희입니다 😊
### 관심있는 분야 : 
-  **보안**: 정보 보안은 모든 시스템의 기초입니다. 보안이 취약하면 아무리 좋은 시스템이라도 신뢰할 수 없습니다. 저는 암호화 기술, 보안 프로토콜, 침입 탐지 시스템 등 다양한 보안 기술에 관심이 많습니다. 특히, AES와 같은 대칭키 암호화 알고리즘과 RSA와 같은 비대칭키 암호화 알고리즘을 활용한 데이터 보호 방법에 대해 공부하는 중입니다. **현재는 칼리 리눅스(Kali Linux)를 활용하여 해킹과 보안 테스트를 공부하고 있으며, 이를 통해 다양한 보안 취약점을 탐지하고 해결하는 방법을 학습하고 있습니다**
-  **스트럭쳐** : 효율적인 소프트웨어 구조는 프로그램의 성능과 유지보수에 큰 영향을 미칩니다. 저는 MVC 패턴, 사가 패턴, DDD(도메인 주도 설계) 구조와 같은 다양한 소프트웨어 아키텍처 패턴에 관심이 많습니다. 이러한 패턴들은 복잡한 시스템을 체계적으로 설계하고, 유지보수를 용이하게 하며, 코드의 재사용성을 높이는 데 중요한 역할을 합니다.
-  **알고리즘** : 효율적인 데이터 구조는 프로그램의 성능을 좌우합니다. 저는 트리, 그래프, 해시 테이블 등 다양한 데이터 구조를 활용하여 복잡한 문제를 해결하는 것에 큰 흥미를 가지고 있습니다. 특히, 그래프 이론과 이를 활용한 네트워크 분석, 최단 경로 찾기 알고리즘 등에 대해 공부하는 것을 좋아합니다.
### 최근 개발한 서비스 (2024년 5월 기준): SettleUp 💵 
### 서비스 소개 :
저희 서비스는 그룹 내 공유 정산서 기능을 제공합니다. 특히 장기간에 걸쳐 자주 발생하는 지출이 있는 경우(룸메이트, 장기 여행자, 정기 모임 등)에 초점을 맞추고 있습니다. </br>
이런 상황에서는 각 거래 후 바로 정산하지 않으면, 시간이 지나면서 누가 누구에게 얼마나 채무가 있는지 파악하기 어려워집니다. 저희 시스템은 이를 해결하기 위해 개발되었습니다.</br>

SettleUp 서비스를 통해 사용자는 영수증 사진을 간편하게 등록할 수 있습니다.</br>
이렇게 쌓인 비용은 최적화 자료에 따라 언제든지 유저가 원하는 시기에 개인적으로 송금하고, 그 결과는 그룹 전체에 반영됩니다. 장기간 비용이 발생하는 모임에서, 모든 거래를 추적할 필요 없이 저희 시스템은 그룹 내 채무 관계를 알고리즘으로 재조정하여 최소한의 거래 횟수를 요구합니다.</br>

저희 사이트는 장기간 발생한 비용으로 인해 복잡해진 채무 관계를 단순화하여,</br>
사용자가 받아야 할 금액과 지불해야 할 금액을 명확하게 제시합니다. 이 기능이 저희 서비스의 핵심입니다.</br>

### 주요 기능 : 
Microsoft Azure의 외부 API를 이용하여 영수증을 파싱하고, 서비스 목적에 맞도록 데이터를 정제합니다. </br>
유저가 사진을 찍어서 올린 영수증을 기반으로 그룹 내 거래의 최소화를 진행합니다.

유저는 영수증 사진을 업로드하기만 하면, 그룹 내 특정 인원을 아이템별로 선택해 각 금액을 할당하고, 서버에서 최적화를 통해 얽힌 채무 관계를 재조정할 수 있습니다.</br>

일부 송금이 완료되면 보낸 유저는 그 금액을 체크하고, 받는 유저는 페이지에 접속했을 때 누구에게 얼마를 받았는지 확인할 수 있습니다.</br>
또한, 그룹 내 비용 발생의 시작점이 되는 영수증은 날짜별로 유저가 추적할 수 있도록 설계했습니다.</br>

그룹 내 최소화 과정에서 Graph Algorithm, DFS, Sorting Algorithm, AES Encryption 알고리즘이 사용되었으며,</br>
그룹 내 유저가 복잡한 계산을 할 필요 없이 자신이 받거나 줘야 할 돈을 명확하게 나타내주는 것이 특징입니다.

해당 프로젝트는 GitHub Action과 AWS의 CodeDeploy, S3, EC2를 통해 CI/CD 파이프라인을 통해 자동 배포가 이루어지며, </br>
시스템의 구조화와 복잡한 코드가 은닉화되어 캡슐화의 원칙을 잘 따르고 있습니다. 무엇보다 에러 핸들링 부분은 코드의 재사용성을 고려하여 설계하였습니다.</br>
자세한 내용을 파악하고자 하는 분은 아래의 링크에 코드와 더불어 자세히 설명되어 있으니 참고 부탁드립니다.<a href="https://github.com/Settle-Up/settle-up-server"><img src="https://img.shields.io/badge/GitHub-007396?style=flat-square&logo=GitHub&logoColor=white&link=https://github.com/donghee9"/></a>

아래는 제 개인 이메일입니다 추가로 문의 할 것이 있으시면 연락바랍니다
<please contact -> <a href="mailto:seodonghee45@naver.com">
  <img src="https://cdn.jsdelivr.net/gh/dmhendricks/signature-social-icons/icons/round-flat-filled/50px/mail.png" alt="Email" title="Send Email" width="30" height="30" />
</a>

please contact-> seodonghee45@naver.com

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=donghee9&layout=donut&theme=merko)](https://github.com/anuraghazra/github-readme-stats)</br>

**Languages & Frameworks**:
![Java_corretto_17](https://img.shields.io/badge/Java_corretto_17-007396?style=flat-square&logo=java&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-FFD23F?style=flat-square&logo=JavaScript&logoColor=white)
![Shell](https://img.shields.io/badge/Shell-A5DD9B?style=flat-square&logo=Shell&logoColor=white)

**Backend Frameworks**:
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-A5DD9B?style=flat-square&logo=Node.js&logoColor=white)

**Databases**:
![MongoDB](https://img.shields.io/badge/MongoDB-78A083?style=flat-square&logo=MongoDB&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-59B4C3?style=flat-square&logo=MySQL&logoColor=white)
![AZSQL](https://img.shields.io/badge/AZSQL-50C4ED?style=flat-square&logo=MySQL&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-EE4266?style=flat-square&logo=Redis&logoColor=white)

**ORM**:
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white)

**Deploy***:
![GithubAction](https://img.shields.io/badge/GithubAction-EE4266?style=flat-square&logo=Github&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF6631?style=flat-square&logo=AWS&logoColor=white)
![CodeDeploy](https://img.shields.io/badge/CodeDeploy-006400?style=flat-square&logo=AWS&logoColor=white)
![EC2](https://img.shields.io/badge/EC2-FF6600?style=flat-square&logo=EC2&logoColor=white)
![S3](https://img.shields.io/badge/S3-A5DD9B?style=flat-square&logo=S3&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoft&logoColor=white)

**External Tools***:
![Sentry](https://img.shields.io/badge/Sentry-EE4266?style=flat-square&logo=Sentry&logoColor=white)
![ngrok](https://img.shields.io/badge/ngrok-1F1E25?style=flat-square&logo=ngrok&logoColor=white)

**Logging**:
![Log4j](https://img.shields.io/badge/Log4j-FF4500?style=flat-square&logo=apache&logoColor=white)

**Security**:
![OAuth2](https://img.shields.io/badge/OAuth2-4285F4?style=flat-square&logo=oauth&logoColor=white)
![BCrypt](https://img.shields.io/badge/BCrypt-FF4500?style=flat-square&logo=security&logoColor=white)


**Utilities**:
![p6spy](https://img.shields.io/badge/p6spy-00ACC1?style=flat-square&logo=database&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-ED8B00?style=flat-square&logo=json-web-tokens&logoColor=white)
![JAXB](https://img.shields.io/badge/JAXB-9C27B0?style=flat-square&logo=java&logoColor=white)
![Mail](https://img.shields.io/badge/Mail-D14836?style=flat-square&logo=gmail&logoColor=white)
![Nodemailer](https://img.shields.io/badge/Nodemailer-007396?style=flat-square&logo=nodemailer&logoColor=white)


---------------------------------------------------------------------------------------------------------------------------
### 레파지토리 구조:
- [![TeamProject](https://img.shields.io/badge/TeamProject-EE4266?style=flat-square&logo=GitHub&logoColor=white)](https://github.com/donghee9?tab=repositories&q=TeamProject&type=&language=&sort=name) - 백앤드 프론트가 모두 배포되어 사용할 수 있는 서비스
- [![SoloProject](https://img.shields.io/badge/SoloProject-3498DB?style=flat-square&logo=GitHub&logoColor=white)](https://github.com/donghee9?tab=repositories&q=SoloProject&type=&language=&sort=name) - 백엔드만 구현이 되어 있는 프로젝트
- Practice - 개발 역량 증진을 위해 연습 레파지토리</br>
- Resources - 리소스 


------------------------------------------------------------------------------
--------------------------------------------------------------------------------
## I'm Donghee Seo, a Backend Developer 😊
#### Areas of Interest:
- **Security**: Information security is the foundation of all systems. If security is weak, no matter how good the system is, it cannot be trusted. I am highly interested in various security technologies such as encryption techniques, security protocols, and intrusion detection systems. Currently, I am studying data protection methods using symmetric key encryption algorithms like AES and asymmetric key encryption algorithms like RSA. I am also studying hacking and security testing using Kali Linux to detect and resolve various security vulnerabilities.
  
- **Structure**: Efficient software architecture greatly impacts the performance and maintainability of programs. I have a strong interest in various software architecture patterns such as MVC, Saga, and Domain-Driven Design (DDD). These patterns play a crucial role in systematically designing complex systems, facilitating maintenance, and enhancing code reusability.
  
- **Algorithms**: Efficient data structures determine the performance of programs. I am very interested in solving complex problems using various data structures such as trees, graphs, and hash tables. In particular, I enjoy studying graph theory, network analysis, and shortest path algorithms.
  
#### Recently Developed Service (as of May 2024): SettleUp 💵
#### Service Introduction:
Our service provides a shared expense ledger function within groups. It focuses on situations where frequent expenses occur over a long period (roommates, long-term travelers, regular meetings, etc.). In such cases, if settlements are not made immediately after each transaction, it becomes difficult to determine who owes whom and how much over time. Our system was developed to solve this issue.

Through the SettleUp service, users can easily upload photos of receipts. The accumulated costs are optimized so users can make personal transfers at any time they wish, and the results are reflected in the entire group. In gatherings where expenses are incurred over a long period, our system algorithmically readjusts debt relationships within the group to require the minimum number of transactions, simplifying the complex debt relationships that arise over time.

#### Main Features:
Parsing receipts using external APIs from Microsoft Azure and refining the data for the service.
Minimizing group transactions based on receipts uploaded by users.
Allowing users to select specific members within the group per item on the receipt and allocate each amount, with the server optimizing and readjusting the intertwined debt relationships.
Once some payments are completed, the sending user can check the amount, and the receiving user can see who paid and how much when they access the page.
Designing receipts, the starting point of group expenses, to be trackable by users by date.
The process of minimization within the group uses Graph Algorithm, DFS, Sorting Algorithm, and AES Encryption Algorithm, clearly showing users the money they need to receive or pay without complex calculations.

The project is automatically deployed through a CI/CD pipeline using GitHub Action, AWS CodeDeploy, S3, and EC2, following the principles of encapsulation by hiding the structured and complex code. Error handling is designed with code reusability in mind. For more details, please refer to the link below where the code is explained in detail:
<a href="https://github.com/Settle-Up/settle-up-server"><img src="https://img.shields.io/badge/GitHub-007396?style=flat-square&logo=GitHub&logoColor=white&link=https://github.com/donghee9"/></a>

For further inquiries, please contact me at my personal email:
<a href="mailto:seodonghee45@naver.com"><img src="https://cdn.jsdelivr.net/gh/dmhendricks/signature-social-icons/icons/round-flat-filled/50px/mail.png" alt="Email" title="Send Email" width="30" height="30" /></a>
please contact -> seodonghee45@naver.com

Repository Structure
 - [![TeamProject](https://img.shields.io/badge/TeamProject-EE4266?style=flat-square&logo=GitHub&logoColor=white)](https://github.com/donghee9?tab=repositories&q=TeamProject&type=&language=&sort=name) - Fully deployed services including both backend and frontend
 - [![SoloProject](https://img.shields.io/badge/SoloProject-3498DB?style=flat-square&logo=GitHub&logoColor=white)](https://github.com/donghee9?tab=repositories&q=SoloProject&type=&language=&sort=name)  - Projects with backend implementations only
 - Practice - Repositories for skill enhancement
 - Resources - Resources
