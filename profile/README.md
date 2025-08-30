# 🏦 쏠쏠해영 (Solsol) – 캠퍼스 금융 플랫폼

**쏠쏠해영(Solsol)**은 대학생들을 위한 올인원 캠퍼스 금융 플랫폼입니다.  
개인 간 정산부터 학생회비 회계 관리, QR 기반 결제와 쿠폰까지 —  
대학 생활 속 모든 **금융 경험을 하나의 앱 안에서 해결**할 수 있도록 설계되었습니다.  

이 Organization에서는 **Android 앱 클라이언트**와 **Spring Boot 기반 Backend**를 함께 관리합니다.  

---

## 📱 [쏠쏠해영 Android 앱](https://github.com/CANSHOOT/solsol-android)

<img width="250" height="600" alt="image" src="https://github.com/user-attachments/assets/d222d07e-f96c-4433-b156-d873d337e3d5" />

Android 앱은 **Kotlin + Jetpack Compose**로 개발되었으며,  
QR 결제, 송금, 정산, 학생회 관리 기능을 제공합니다.  

- QR 결제 + 지문 인증 보안  
- 그룹/개인 송금 및 푸시 알림  
- 균등/직접입력/랜덤게임 기반 정산  
- 학생회비 관리 + OCR 영수증 인식  
- 실시간 알림 (Firebase FCM)  

👉 [solsol-android 레포로 이동하기](https://github.com/CANSHOOT/solsol-android)

---

## 🏃‍♂️ [Solsol Backend](https://github.com/CANSHOOT/solsol-backend)

Backend는 **Spring Boot + MySQL**을 기반으로 하며,  
특히 **출석률 기반 자동 쿠폰 발급 시스템**을 포함한 다양한 배치/스케줄링 로직을 제공합니다.  

- 매일 새벽 3시 10분 자동 쿠폰 발급  
- 출석률 구간별 차등 보상 지급  
- Jasypt 암호화 & JWT 기반 인증  
- 멀티 프로필 (개발/운영) 지원
- 대용량 배치 처리: 10,000건씩 페이징, 1,000건마다 메모리 최적화
- 중복 발급 방지: 당일 이미 발급된 사용자 제외, 키셋 페이징으로 효율적 처리

👉 [solsol-backend 레포로 이동하기](https://github.com/CANSHOOT/solsol-backend)

---

## 🛠️ 기술 스택

- **Android**: Kotlin, Jetpack Compose, MVVM, Hilt, Retrofit, Room, CameraX, ML Kit(OCR), Biometric API, Firebase FCM  
- **Backend**: Java 21, Spring Boot 3.x, MySQL 8.x, QueryDSL, JPA, Scheduler, Jasypt, JWT  
- **공통**: REST API, OAuth2 인증, CI/CD (Gradle + GitHub Actions 예정)

---

## 🚀 프로젝트 구조
```
organization/
├── solsol-android/ # Android 클라이언트 (Kotlin, Compose)
└── solsol-backend/ # Spring Boot Backend (쿠폰 발급, 정산/송금 API)
```

---

## 📌 비전

쏠쏠해영은 단순한 금융 앱이 아니라,  
**대학생의 일상 속 불편을 해소하고, 학생회와 학생 간 신뢰를 강화하며,  
캠퍼스 경제 생태계를 하나로 연결하는 플랫폼**을 지향합니다.  

---

🔗 지금 바로 확인해보세요!  
- [solsol-android 바로가기](https://github.com/CANSHOOT/solsol-android)  
- [solsol-backend 바로가기](https://github.com/CANSHOOT/solsol-backend)  
