# 🍪 MOMS Cookie : 아침이 두려운 당신을 위해, 엄마처럼 챙겨주는 스마트 알람 비서

<div align="center">
  <p>더이상의 "5분만 더"는 없다</p>
</div>

---

## 🧠 프로젝트 소개

**MOM's Cookie는** 센서, AI, Wi-Fi 연동 기능을 갖춘 스마트 알람 시스템으로, 바쁜 현대인의 아침을 자동화해주는 IoT 기반의 AI 비서 프로젝트입니다.
하드웨어와 소프트웨어를 통합하여, 사용자의 아침 루틴을 자동화하고 최적화합니다.

---

## 💡 주요 기능

- 🧠 **AI 비서 (GPT-4 Turbo 기반)**  
  음성으로 질문하면 일정, 날씨, 맞춤형 조언을 제공합니다.

- ⏰ **스마트 알람 & 장치 제어**  
  알람이 울리면 조명과 보일러가 자동 제어되며, 습도에 따라 가습기가 동작합니다.

- 📅 **일정 관리 및 정보 알림**  
  당일 중요 일정을 정리해 알려주고, 날씨/미세먼지 정보도 함께 안내합니다.

- 📡 **Wi-Fi 통신 기반 시스템 연동**  
  ESP32를 사용한 안정적인 서버 연동으로 다양한 모듈들과 통신합니다.

---

##  🛠️ 사용 기술들

✅ 프로그래밍 언어

<img src="https://img.shields.io/badge/c++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white"> <img src="https://img.shields.io/badge/c-A8B9CC?style=for-the-badge&logo=c&logoColor=white"> <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white">

✅ 임베디드 & 하드웨어

<img src="https://img.shields.io/badge/arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white"> <img src="https://img.shields.io/badge/stm32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white"> <img src="https://img.shields.io/badge/raspberry%20pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white"> <img src="https://img.shields.io/badge/turtlebot3-22314E?style=for-the-badge&logo=ros&logoColor=white">

✅ 플랫폼 & 프레임워크

<img src="https://img.shields.io/badge/ROS-22314E?style=for-the-badge&logo=ros&logoColor=white"> <img src="https://img.shields.io/badge/flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white"> <img src="https://img.shields.io/badge/openai-412991?style=for-the-badge&logo=openai&logoColor=white"> <img src="https://img.shields.io/badge/openapi-6BA539?style=for-the-badge&logo=openapiinitiative&logoColor=white">

✅ 빌드 & 개발 환경

<img src="https://img.shields.io/badge/cmake-064F8C?style=for-the-badge&logo=cmake&logoColor=white"> <img src="https://img.shields.io/badge/ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white">

---

## 🧱 시스템 구성도

```
[사용자 음성 입력]
        ↓
[ESP32 Wi-Fi] ←→ [Flask API 서버] ←→ [GPT-4 Turbo]
        ↓
[STM32, Arduino Mega, 센서 및 액추에이터]
        ↓
[알람 / 조명 / 보일러 / 가습기 제어]
```

---

## 📁 프로젝트 구조

```plaintext
project_MOMs_Cookie/
├── App/
│   └── calendar/                # 일정 관리 모듈
├── BUZZER/                      # 알람 기능 구현
├── GPT4_Turbo/                  # AI 비서 기능
├── sensor_led/                  # 센서 및 LED 제어 (STM32 기반)
├── wifi_module_arduinomega/     # Wi-Fi 통신 모듈 (Arduino Mega 기반)
├── 서버 및 브릿지(API)/
│   └── final/                   # API 서버 및 브릿지 구현
├── 시연영상/                    # 프로젝트 시연 영상
└── 회로도/                      # 하드웨어 회로도
```

---

## 📽️ 시연 영상

시연 영상은 [여기](https://github.com/k-tae/project_MOMs_Cookie/tree/main/%EC%8B%9C%EC%97%B0%EC%98%81%EC%83%81)에서 확인하실 수 있습니다.

---

## 📄 회로도

하드웨어 회로도는 [여기](https://github.com/k-tae/project_MOMs_Cookie/tree/main/%ED%9A%8C%EB%A1%9C%EB%8F%84)에서 확인하실 수 있습니다.

---

## 개발자
<div align="center">

|권태형(팀장)|이종범(부팀장)|임소연|김병성|
|:------:|:------:|:------:|:------:|
| <a href="https://github.com/k-tae"><img width="150px" style="max-width: 100%;" src="https://github.com/k-tae.png"></a> | <a href="https://github.com/whdqja1128"><img width="150px" style="max-width: 100%;" src="https://github.com/whdqja1128.png"></a> | <a href="https://github.com/imso01"><img width="150px" style="max-width: 100%;" src="https://github.com/imso01.png"></a> | <a href="https://github.com/kimbseong0814"><img width="150px" style="max-width: 100%;" src="https://github.com/kimbseong0814.png"></a> |

</div>

---

## 🎯 기대 효과 및 향후 목표

- 효율적인 아침 준비로 **시간 절약**과 **스트레스 감소**
- **음성 AI + IoT 통합 플랫폼**으로 확장 가능성 확보
- 향후 목표:
  - 사용자 맞춤 DB 기반 추천 시스템 구축
  - 냉장고/신발장/우산 인식 및 알림 기능 연동
  - 회원가입 기능 및 멀티 사용자 관리 시스템 개발

---

---

## 📬 문의

이슈를 통해 문의를 남겨주시거나, 각 개발자에게 직접 연락 바랍니다.
