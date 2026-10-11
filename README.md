# Jeonghan Lee | 이정한

**Embedded Linux · C/C++ · Device Drivers · Qt · HW/SW Integration**

안녕하세요. 하드웨어의 동작을 이해하고, Linux 시스템부터 응용 소프트웨어까지 연결하는 개발에 관심이 있습니다.

제어계측공학을 전공했으며, **한화비전 VEDA 3기**에서 임베디드 Linux, 디바이스 드라이버, C++/Qt, 영상관제 시스템 개발과 통합을 경험했습니다.

## Technical Skills

| Area | Technologies |
| --- | --- |
| Languages | C, C++ |
| Embedded / Linux | Linux Kernel Module, Character Device Driver, Raspberry Pi, GPIO, PWM, ARM64 Cross Compilation |
| Application / Network | Qt Widgets, TCP/IP Socket, POSIX Threads, Shared Library (`dlopen` / `dlsym`) |
| Build / Collaboration | CMake, Makefile, Jenkins CI/CD, Git, Jira, Confluence |

## Selected Projects

### 1. RoadSide — WISE AI 기반 갓길 주정차 관제 시스템

**한화비전 VEDA 3기 Final Project 최우수상 · 4인 팀장**

한화비전 AI CCTV 4대와 Qt 기반 영상관제 프로그램, 주차 상태 관리, Raspberry Pi 컨트롤러를 연동한 팀 프로젝트입니다.

**직접 담당한 업무**
- Raspberry Pi 기반 **VMS Hardware Controller** 및 터치스크린용 Qt GUI 개발
- Linux 입력장치 인터페이스와 GPIO를 활용한 조이스틱·버튼·로터리 엔코더 입력 처리
- 입력을 TCP 제어 명령으로 변환하여 VMS 채널 전환·Software PTZ·기능 버튼과 연동
- **Software PTZ 직접 구현**, Polygon ROI 기능 공동 구현
- Jenkins 기반 Windows 빌드·패키징·배포 자동화
- 프로젝트 일정 조율, 기능 통합 및 최종 발표

**팀 저장소:** [RoadSide Qt VMS Application](https://github.com/VEDA-Final-Project/veda_QT)

> 팀 저장소에는 다른 팀원의 개발 결과도 포함되어 있습니다. 위 항목은 제 담당 업무를 별도로 구분한 내용입니다.

### 2. Project Tankboy — Linux Character Device Driver 기반 RC Tank

**VEDA 프로젝트 경진대회 우승 · Linux Kernel / Hardware Control**

Raspberry Pi에서 동작하는 원격 RC Tank 팀 프로젝트입니다.

**직접 담당한 업무**
- L298 듀얼 모터의 배선·전원 구성과 실물 하드웨어 조립
- `/dev/tankmotor` Character Device Driver 구현
- `ioctl` 기반 모터 속도·방향 명령 전달
- `hrtimer` 기반 Software PWM 및 `spinlock`을 활용한 공유 상태 보호
- GPIO Mapping 및 커널 빌드 환경 문제 해결, 실제 구동 테스트

**소스 코드:** [Tankboy DeviceDriver (kernel module & test app)](https://github.com/veda-car-project/DeviceDriver)

> 공개 팀 저장소 중 제가 직접 작성한 Linux 모터 드라이버 및 테스트 앱 코드입니다. 팀 전체 RC Tank 응용 프로그램과는 구현 범위가 다릅니다.


### 3. VeraCalendar — Qt Desktop Application

**C++17 · Qt 6 Widgets · 2인 팀 프로젝트**

일정 조회·검색·편집 기능을 결합한 데스크톱 애플리케이션입니다.

**직접 담당한 업무**
- `LeftList`: 미래 일정 조회·정렬·날짜 선택
- `SearchEngine`: 키워드 검색·결과 정렬
- `ToolBox`: 초기화·종료 이벤트
- `MainWindow`: 팀원과 공동으로 Signal/Slot 및 UI 상태 동기화 통합

**관련 팀 저장소:** [midCalender — Qt 캘린더 실습 코드](https://github.com/acoddi/midCalender)

## Training & Practice

### Remote Device Control — VEDA Linux 시스템 프로그래밍 실습

**교육 과정에서 수행한 Linux 실습 과제**

Ubuntu Client와 Raspberry Pi Server 사이의 TCP 통신을 통해 LED, Buzzer, 조도센서, 7-Segment 장치 제어를 연습했습니다.

**실습 내용**
- POSIX Socket 기반 Client/Server 통신과 `pthread` 활용
- `dlopen` / `dlsym`으로 Shared Library와 Device Layer 연동
- Mutex를 활용한 동기화, Daemon 실행 및 ARM64 Cross Compilation

---

**Areas of Interest:** Embedded Linux · Linux Device Drivers · C/C++ · Qt · Hardware/Software Integration
