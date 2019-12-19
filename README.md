# ci-cd-practice

## SW 개발 프로세스

> 폭포수 모겔링: 분석, 설계, 개발, 구현, 시험, 유지보수과정을 순차적으로 접근하는 방법
>> 가장 오래된 방법론
>> 시간 소요가 많은 단점이 있다.

> 애자일 방법론
>> TDD, Scrum, XP, Kanban, sprint, etc.

> Kanban
>> 단순 -> 스테이지 -> WIP와 Queue

> DevOps
>> 개발과 운영을 합친 용어
>> 개발과 운영 간의 상호 작용을 원활하게 하는 모든 것을 의미하는 포괄적인 개념
>> 부서 간 통합, 커뮤니케이션, 협업을 강조
>> 지속적 환경이 유지되는 Cycle을 자동화
>
> 폭포수 모델에서 애자일로 변환되고 있다.

> Jira
>> 프로젝트 생성 -> 이슈 생성 -> 워크플로우 관리 -> 대시보드 -> 검색 및 리포트
>> OPEN -> IN PROGRESS -> RESOLVED -> CLOSED / REOPENED
> 
> 애자일보드
>> 스크럼, 칸반 보드 지원
>
> Confluence


## CI

1. 버전관리 저장소
2. 지속적인 통합서버
3. 빌드 스크립트
4. Project Management Tool - email, SNS, slack


## CD

> release 가능한 package까지 만드는 것
> CI + Quality Management Tool
>
> 보통의 경우 CI 까지 자동화하고, 개발단계를 진행하며 Delevery, 배포는 승인을 통해 이루어 진다.
>
> Jenkins: CI 도구
> local 환경 개발 도구: Docker
>
> compile - build - test - packaging - release


## Jenkins - Slack 연동

> Jenkins 관리 -> 플러그인 관리 -> 설치 가능 탭에서 slack 설치
> Job -> 빌드 후 조치 -> Slack Notifications 등록
>
> 1. 새로운 item 설정, freestyle로 셍성
> 2. 소스코드 git 설정, 빌드 Invoke top - level Maven target 설정
>
> 활용방안
>> 1. Spring Batch Admin
>> 2. Health Check
>> 3. Watch Dog(System Monitoring)
>> 4. ACL Checker
>> 5. IaC Execute & Schedule



